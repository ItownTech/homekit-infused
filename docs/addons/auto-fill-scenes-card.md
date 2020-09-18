# Homekit Infused

Back to [Addon List](../addon_list.md)

# Auto Filled Scenes Card
*HKI Framework 3.0.2 or higher required

![Homekit Infused](../images/auto-fill-scenes-card.png)

### Description
This is a card that will fetch all your scenes and create a button page for it automatically

### Configuration
- No additional config required

### Advanced

| Properties | Required | Default | Description |
|----------------------------------|-------------|----------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| column_num | no | 1 | Sets how many battery entities should be stacked horizontally on each column |
| method | no | name | Sorts the cards in a different order, choose from: domain, entity_id, name, state, attribute, last_changed last_updated or last_triggered |
| other | | | It is probably best if you leave all the other settings alone! |
| grid | no | '!include ../../../base/includes/default-hki-grid.yaml' | Change the grid (best to leave this alone if you don't know what the grid is for) |

### Install
- Create a new file inside the folder of the view you want (e.g. /homekit-infused/user/views/scenes/), you can name the file however you want (e.g. scenes-card.yaml)
- Copy the code below and make changes if needed

```
- type: horizontal-stack
  cards:
    - !include ../../../base/includes/gap.yaml
    - type: custom:auto-entities
      filter:
        include:
          - domain: scene
            options:
              !include
              - '../../../base/templates/button/service-call.yaml'
              - entity: this.entity_id
                grid:
                  '!include ../../../base/includes/light-devices-grid.yaml'
                service_entity: this.entity_id
                show_state: false
          - type: custom:button-card
            color_type: blank-card
            aspect_ratio: 1/1
          - type: custom:button-card
            color_type: blank-card
            aspect_ratio: 1/1
      sort:
        method: name
        numeric: true
      card:
        type: custom:layout-card
        column_num: 3
        justify_content: start
        layout: horizontal
    - !include ../../../base/includes/gap.yaml
```

