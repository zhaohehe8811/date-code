# date-code
date area
import { DatePicker } from 'antd';
import moment from 'moment';
const { MonthPicker, RangePicker } = DatePicker;

const dateFormat = 'YYYY/MM/DD';
const monthFormat = 'YYYY/MM';
ReactDOM.render(
  <div>
    <DatePicker defaultValue={moment('2017/04/05', dateFormat)} format={dateFormat} />
    <br />
    <MonthPicker defaultValue={moment('2017/08', monthFormat)} format={monthFormat} />
    <br />
    <RangePicker
      defaultValue={[moment('2017/04/01', dateFormat), moment('2017/08/01', dateFormat)]}
      format={dateFormat}
    />
  </div>
, mountNode);
