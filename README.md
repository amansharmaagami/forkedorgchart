## This library is forked version of [this](https://github.com/dabeng/react-orgchart) library with some extra layers




## Features
- expand/collapse nodes
- Allows user to change orgchart structure by drag/drop nodes
- Allows user to edit orgchart
- Supports exporting chart as a picture or pdf document
- Supports pan and zoom
- Allows user to customize the internal structure for every node

## Props
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Type</th>
      <th>Default</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>chartClass</td>
      <td>string</td>
      <td></td>
      <td>A css class to apply to the chart DOM node.</td>
    </tr>
    <tr>
      <td>containerClass</td>
      <td>string</td>
      <td></td>
      <td>Add an optional extra class name to .orgchart-container It could end up looking like class="orgchart-container xxx yyy".</td>
    </tr>
    <tr>
      <td>collapsible</td>
      <td>boolean</td>
      <td>true</td>
      <td>Allows expanding/collapsing the nodes.</td>
    </tr>
    <tr>
      <td>datasource</td>
      <td>object</td>
      <td></td>
      <td>datasource usded to build out structure of orgchart.</td>
    </tr>
    <tr>
      <td>draggable</td>
      <td>boolean</td>
      <td>false</td>
      <td>Allows dragging/dropping the nodes to the hierarchy of chart.</td>
    </tr>
    <tr>
      <td>multipleSelect</td>
      <td>boolean</td>
      <td>false</td>
      <td>If true, user can select multiple nodes by mouse clicking.</td>
    </tr>
    <tr>
      <td>NodeTemplate</td>
      <td>elementType</td>
      <td></td>
      <td>A Component that provides the node content Markup. This is a useful prop when you want to use your own styles and markup to create a custom orgchart node.</td>
    </tr>
    <tr>
      <td>onClickChart</td>
      <td>function</td>
      <td></td>
      <td>A callback fired when the orgchart is clicking.</td>
    </tr>
    <tr>
      <td>onClickNode</td>
      <td>function</td>
      <td></td>
      <td>A callback fired when the node is clicking.</td>
    </tr>
    <tr>
      <td>pan</td>
      <td>boolean</td>
      <td>false</td>
      <td>If true, the chart can be panned.</td>
    </tr>
    <tr>
      <td>zoom</td>
      <td>boolean</td>
      <td>false</td>
      <td>If true, the chart can be zoomed.</td>
    </tr>
    <tr>
      <td>zoominLimit</td>
      <td>number</td>
      <td>7</td>
      <td>User can zoom the chart at different scales(0.5~7).</td>
    </tr>
    <tr>
      <td>zoomoutLimit</td>
      <td>number</td>
      <td>0.5</td>
      <td>User can zoom the chart at different scales(0.5~7).</td>
    </tr>
    <tr>
      <td>onDropZone</td>
      <td>function</td>
      <td></td>
      <td>
        A Callback fired  when the node drop at targeted node.
        Will recieve two params first is node which is dragged,
        second param will be the targeted node id property
      </td>
    </tr>
  </tbody>
</table>

## Methods
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>expandAllNodes</td>
      <td>User can use this method to expand all the nodes. Sample code: orgchartRef.current.expandAllNodes()</td>
    </tr>
    <tr>
      <td>exportTo</td>
      <td>User can use this method to export orgchart to png org pdf file. Sample code: orgchartRef.current.exportTo(filename, fileextension)</td>
    </tr>
  </tbody>
</table>


## Install
```
npm install forkedorgchart
```
