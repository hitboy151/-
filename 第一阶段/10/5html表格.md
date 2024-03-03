# 表格(table)
- 在网页中可以创建表格表示格式化的数据
- 在html中使用table创建一个表格
  - 
  ```
  <table>
    <caption></caption>//表格标题
    <thead>//表头
        <tr>//表示一行
            <th></th>//表示表头单元格，自动加粗居中
            <td></td>//表示一格
            <td></td>
        </tr>
    </thead>
    <tbody>//表中
    </tbody>
    <tfoot>//表尾
    </tfoot>
  </table>
  ```
- `border-collapse`(css)
  - 设置表格边框合并
  - 设置为collapse表示合并
  - 默认不合并
- `colspan`合并横向单元格(td属性)
  - `<td colspan="3"></td>//合并从自己到左边3个单元格`
- `rospan`合并纵向单元格(td属性)
- 表头表尾和表头书写位置和显示位置无关
- table中没有设置表头表中表尾直接设置单元，则浏览器自动生成tbody 
- 文字在td中会自动垂直居中
- `vertical-align:middle;`在单元格中使得文字垂直居中
- `display:table-cell;`把元素转化为单元格