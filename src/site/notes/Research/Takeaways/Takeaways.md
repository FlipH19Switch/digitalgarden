---
{"dg-publish":true,"permalink":"/research/takeaways/takeaways/"}
---


```yaml:dbfolder
name: new database
description: new description
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 1
    isHidden: false
    sortIndex: -1
    width: 253
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      wrap_content: true
  __created__:
    key: __created__
    id: __created__
    input: metadata_time
    label: Created
    accessorKey: __created__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: true
    position: 11
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  __modified__:
    key: __modified__
    id: __modified__
    input: metadata_time
    label: Modified
    accessorKey: __modified__
    isMetadata: true
    isDragDisabled: false
    skipPersist: false
    csvCandidate: true
    position: 10
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Takeaways__Level_2_Insights:
    input: relation
    accessorKey: Takeaways__Level_2_Insights
    key: Takeaways__Level_2_Insights
    id: Level_2_Insights
    label: Level 2 Insights
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 108
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      wrap_content: true
      relation_color: hsl(0,0%,0%)
      related_note_path: Research/Level 2 Insights/Level 2 Insights.md
      bidirectional_relation: true
  Takeaways__Level_3_Insights:
    input: relation
    accessorKey: Takeaways__Level_3_Insights
    key: Takeaways__Level_3_Insights
    id: Level_3_Insights
    label: Level 3 Insights
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 135
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      wrap_content: true
      relation_color: hsl(0,0%,0%)
      related_note_path: Research/Level 3 Insights/Level 3 Insights.md
      bidirectional_relation: true
  Takeaways__Assumptions:
    input: relation
    accessorKey: Takeaways__Assumptions
    key: Takeaways__Assumptions
    id: Assumptions
    label: Assumptions
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      wrap_content: true
      relation_color: hsl(0,0%,0%)
      related_note_path: Research/Assumptions/Assumptions.md
      bidirectional_relation: true
  Takeaways__Level_1_Insights:
    input: relation
    accessorKey: Takeaways__Level_1_Insights
    key: Takeaways__Level_1_Insights
    id: Level_1_Takeaways
    label: Level 1 Insights
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      wrap_content: true
      relation_color: hsl(0,0%,0%)
      related_note_path: Research/Level 1 Insights/Level 1 Insights.md
      bidirectional_relation: true
  Takeaways__Actions:
    input: relation
    accessorKey: Takeaways__Actions
    key: Takeaways__Actions
    id: Supporting_Takeaways
    label: SUPPORTED ACTIONS
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      wrap_content: true
      relation_color: hsl(240,100%,1%)
      related_note_path: Research/Actions/Actions.md
      bidirectional_relation: true
  Takeaways__Tags:
    input: relation
    accessorKey: Takeaways__Tags
    key: Takeaways__Tags
    id: Tags
    label: Tags
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      wrap_content: true
      relation_color: hsl(240,100%,1%)
      related_note_path: Research/Tags/Tags.md
      bidirectional_relation: true
  Added_to_Blog:
    input: checkbox
    accessorKey: Added_to_Blog
    key: Added_to_Blog
    id: Added_to_Blog
    label: Added to Blog
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Takeaways__Level_4_Insights:
    input: relation
    accessorKey: Takeaways__Level_4_Insights
    key: Takeaways__Level_4_Insights
    id: Level_4_Insights
    label: Level 4 Insights
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      content_alignment: text-align-left
      wrap_content: true
      relation_color: hsl(240,100%,1%)
      related_note_path: Research/Level 4 Insights/Level 4 Insights.md
      bidirectional_relation: true
  test:
    input: relation
    accessorKey: test
    key: test
    id: test
    label: test
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      related_note_path: Research/Actions/Actions.md
config:
  remove_field_when_delete_column: false
  cell_size: normal
  sticky_first_column: true
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: true
  show_metadata_modified: true
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 200
  font_size: 14
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: bottom
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: false
  conditions:
```