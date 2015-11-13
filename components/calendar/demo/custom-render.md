# 自定义渲染

- order: 1

用 `dateCellRender` 和 `monthCellRender` 函数来自定义需要渲染的数据。

---

````jsx
import { Calendar } from 'antd';

function dateCellRender(value) {
  return <div>自定义日数据</div>;
}

function monthCellRender(value) {
  return <div>自定义月数据</div>;
}

ReactDOM.render(
  <Calendar value={new Date('2010-10-10')}
  dateCellRender={dateCellRender} monthCellRender={monthCellRender} />
, document.getElementById('components-calendar-demo-custom-render'));
````