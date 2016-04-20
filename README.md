# jquery.bootstrap.validate���

---

�ò����jquery.validate����֤����ʾ������Ϣ������Bootstrap���tooltip���ܴ��棬ʹ��֤��������ۡ�

![View]()

## Dependencies

��ͨ��JQuery������.  

- [jQuery v2.1.3 (>= 1.9.0)](http://jquery.com/)
- [Bootstrap v3.3.4](http://getbootstrap.com)
 
## Getting Started

[����]()

### Usage

������������ʽ�ļ���js�ļ�.

```html
<!-- Required Stylesheets -->
<link href="QueryDialog.css" rel="stylesheet">

<!-- Required Javascript -->
<script src="jquery.js"></script>
<script src="QueryDialog.js"></script>
```

�������������ʽ��DOM�����ҳ��ԭ��û�У���������ҳ���Զ��������DOM.

```html
<div id="QueryDialog"></div>
```

�����÷�����.

```javascript
$(document).ready(function () {
    var arrStr = '[{"queryfieldtype":"1","queryfieldname":"age","queryfieldrmk":"����"},{"queryfieldtype":"6","queryfieldname":"name","queryfieldrmk":"����"},{"queryfieldtype":"5","queryfieldname":"ismarried","queryfieldrmk":"�Ƿ��ѻ�"},{"queryfieldtype":"4","queryfieldname":"birthday","queryfieldrmk":"��������"}]';
    $("#QueryDialog").QueryDialog({ data: arrStr });
});

function test() {
    $("#QueryDialog").show();
    $(".qdialog-mask").show();
}
```

## Data Structure

������һ���ַ������ṹʾ����

```javascript
var arrStr = '[{"queryfieldtype":"1","queryfieldname":"age","queryfieldrmk":"����"},{"queryfieldtype":"6","queryfieldname":"name","queryfieldrmk":"����"},{"queryfieldtype":"5","queryfieldname":"ismarried","queryfieldrmk":"�Ƿ��ѻ�"},{"queryfieldtype":"4","queryfieldname":"birthday","queryfieldrmk":"��������"}]';

//����arrStr��һ��������ַ���������Ὣ��ת��json��ʽ������һ������
//ÿһ����������ṹ��{"queryfieldtype":"1","queryfieldname":"age","queryfieldrmk":"����"}��
//1��queryfieldtype��ʾ��ѯ�����Ĳ������ͣ��硰�����������ַ��͡����������͡��ȣ����1��������ǡ����������֡�����ȻҲ���Ը���ʵ���������Լ����
//2��queryfieldname��ʾ��ѯ�������ֶ����ƣ���Ҫ���ĸ��ֶν��й��ˣ�
//3��queryfieldrmk��ʾ��ѯ�����ֶε���ʾ���ƣ�
```