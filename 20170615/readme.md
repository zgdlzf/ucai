# 1. 表单2
## form
form内部单选 复选 下拉菜单多加required
## 1.1. select
### 1.1.1. option 元素
### 1.1.2. select属性包括： size为1时是下拉菜单，超过1时是滚动列表 multiple 
### 1.1.3. option属性 selected属性 disabled
### 1.1.4. 通用属性
required 给有name的标签
### datalist 必须和input结合使用，input中list属性必须是datalist的id。datalist名字在input中给出。datalist中的option没有结束标签
```
        <select name="city" size="10" multiple required>
            <option value="0">北京</option>
            <option value="1" disabled>深圳</option>
            <option value="2">成都</option>
            <option value="3">武汉</option>
            <option value="4">杭州</option>
        </select>
        <input type="submit" value="提交">
        <input type="text" class="" list="data" name="city">
        <datalist id="data">
            <option value="beijing">
            <option value="shanghai">
            <option value="shenzhen">
            <option value="guangzhong">
            <option value="hangzhou">
        </datalist>
```
### fieldset 
分组对表单控件分组
#### legend与fieldset搭配使用，显示分组的标题