# jquery.bootstrap.validate���

---

�ò����jquery.validate����֤����ʾ������Ϣ������Bootstrap���tooltip���ܴ��棬ʹ��֤��������ۡ�

![View](https://github.com/aphy358/jquery.bootstrap.validate/blob/master/screenshot1.jpg)

## Dependencies

��ͨ��JQuery������.  

- [jQuery v2.1.3 (>= 1.9.0)](http://jquery.com/)
- [Bootstrap v3.3.4](http://getbootstrap.com)
 

## Getting Started

### Usage

������������ʽ�ļ���js�ļ�.

```html
<!-- Required Stylesheets -->
<link href="./css/QueryDialog.css" rel="stylesheet">
<link href="./css/jquery.validate.css" rel="stylesheet">

<!-- Required Javascript -->
<script src="./js/jquery.js"></script>
<script src="./js/bootstrap.min.js"></script>
<script src="./js/jquery.validate.js"></script>
```

�����÷�����ȥ���ϲ���jquery.validate��������ϣ������о�ʾ������.

```javascript
$(document).ready(function () {
    InitValidator();            //����Ҫ��ʼ����֤
});

//��ʼ����֤
function InitValidator() {
    $("form").validate({
	rules: {
	    mobile: {
		mobile: true,
	    },
	    date: {
		required: true,
	    },
	},
    });
};

$(".query-go").on("click", function () {
    if (!$("form").iboValid()) return;		//���ύ��֮ǰ������֤
});
```

## Tips

�ò����Ҫ���޸���jquery.validate�е�showErrors��������ʾ������Ϣ��tooltip�ķ�ʽ��

�������ﲢû��ʹ��Bootstrap��ԭ����ʽ�ļ���100��K�����ֻ��˵�ʹ���ǲ���̫�������ˡ�

����ֻ�ǽ����õ��Ĳ��ֽ�ȡ�������ѡ�