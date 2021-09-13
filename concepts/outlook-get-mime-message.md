---
title: Получение содержимого MIME сообщения
description: Multipurpose Internet Mail Extensions (MIME) — это отраслевой стандарт электронной почты. Теперь вы можете использовать сегмент `$value`, чтобы получить содержимое MIME из сообщения Outlook.
author: abheek-das
ms.localizationpriority: high
ms.prod: outlook
ms.openlocfilehash: 541c2481c8534cec7f96010a55beb6d02d825a62
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59135937"
---
# <a name="get-mime-content-of-a-message"></a>Получение содержимого MIME сообщения

MIME — это отраслевой стандарт электронной почты. Многие приложения электронной почты создают сообщения в формате MIME и сохраняют их в файлах с расширением .EML. 

Несмотря на то что Outlook _не сохраняет_ сообщения в формате MIME, текст сообщения Outlook в формате MIME можно получить двумя способами:

- Вы можете добавить сегмент `$value` к операции get-message с этим сообщением.
- Если сообщение вложено в элемент Outlook или запись в группе, вы можете добавить сегмент `$value` к операции get-attachment с этим элементом или записью.

В любом случае приложению должны быть предоставлены [разрешения на доступ](permissions-reference.md#mail-permissions) к элементу Outlook или записи, чтобы применить операцию get-message или get-attachment. 

Затем вы можете сохранить содержимое текста сообщения в EML-файле и вкладывать файл в записи в бизнес-системах, например для CRM, ERP и отслеживания ошибок. 


## <a name="what-is-mime"></a>Что такое MIME?

MIME — это стандарт, используемый для электронной почты в Интернете, чтобы передавать контент следующих типов по протоколу SMTP: 

- сообщение в формате обычного текста;
- сообщение с альтернативным содержимым (т. е. с обычным текстом и HTML);
- ответ, в который вложено исходное сообщение;
- текстовое сообщение с вложенными изображениями, звуковыми файлами, видео или файлами приложений;  
- другие конструкции сообщений.

Ниже представлены типичные заголовки MIME в сообщении. Дополнительные сведения см. в статье [RFC 2045](https://tools.ietf.org/html/rfc2045).

- `MIME-Version` — указывает, что сообщение представлено в формате MIME.
- `Content-Type` — указывает тип мультимедиа сообщения или его части, представленный свойствами *type* и *subtype*. Он также включает поле `boundary`, указывающее строку в виде границы MIME или границы инкапсуляции (в зависимости от расположения `Content-Type`). 
- `Content-Disposition` — предоставляет сведения о вложении, например стиль его отображения (`inline` или `attachment`), имена файлов, а также даты создания и последнего изменения.
- `Content-Transfer-Encoding` — указывает метод шифрования, используемый для представления двоичных данных.

## <a name="get-mime-content-of-an-outlook-message"></a>Получение содержимого MIME сообщения Outlook

Вы можете получить представление сообщения в формате MIME, добавив сегмент `$value` при [получении сообщения](/graph/api/message-get?view=graph-rest-1.0): 

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/messages/{id}/$value
```

### <a name="example"></a>Пример

Ниже приведен пример, в котором запрашивается возврат сообщения из почтового ящика вошедшего пользователя вместе с его содержимым в формате MIME.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

Ниже приведен отклик. Содержимое MIME начинается с заголовка `MIME-Version`. 

<!-- { "blockType": "ignored" } -->
```http
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0 via Mailbox 
Transport; Mon, 4 Sep 2017 03:00:08 -0700 
Received: from contoso.com (10.194.241.197) by 
contoso.com (10.194.241.197) with Microsoft 
SMTP Server (version=TLS1_2, 
cipher=TLS_ECDHE_RSA_WITH_AES_256_CBC_SHA384_P256) id 15.1.1374.0; Mon, 4 Sep 
2017 03:00:07 -0700 
Received: from contoso.com 
(fe80::5bf:5059:4ca0:5017) by contoso.com 
(fe80::5bf:5059:4ca0:5017%12) with mapi id 15.01.1374.000; Mon, 4 Sep 2017 
03:00:01 -0700 
From: Administrator <admin@contoso.com> 
To: Administrator <admin@contoso.com> 
Subject: This email has attachment. 
Thread-Topic: This email has attachment. 
Thread-Index: AQHTJWSHSywMzSz8o0OJud48nG50GQ== 
Date: Mon, 4 Sep 2017 10:00:00 +0000 
Message-ID: 
                <4aade2547798441eab5188a7a2436bc1@contoso.com> 
Accept-Language: en-US 
Content-Language: en-US 
X-MS-Exchange-Organization-AuthAs: Internal 
X-MS-Exchange-Organization-AuthMechanism: 04 
X-MS-Exchange-Organization-AuthSource: 
                contoso.com 
X-MS-Has-Attach: yes 
X-MS-Exchange-Organization-Network-Message-Id: 
                0ffdb402-ec03-42c8-5d32-08d4f37bb517 
X-MS-Exchange-Organization-SCL: -1 
X-MS-TNEF-Correlator: 
X-MS-Exchange-Organization-RecordReviewCfmType: 0 
x-ms-publictraffictype: Emai

```http
MIME-Version: 1.0 
Content-Type: multipart/mixed; 
                boundary="_004_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: multipart/alternative; 
                boundary="_000_4aade2547798441eab5188a7a2436bc1contoso_" 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/plain; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
The attachment is an email. 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: text/html; charset="iso-8859-1" 
Content-Transfer-Encoding: quoted-printable 
 
<html> 
<head> 
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-= 
1"> 
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi= 
n-bottom:0;} --></style> 
</head> 
<body dir=3D"ltr"> 
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font= 
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr"> 
<p>The attachment is an email.</p> 
</div> 
</body> 
</html> 
 
--_000_4aade2547798441eab5188a7a2436bc1contoso_-- 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_ 
Content-Type: application/octet-stream; name="Attachment email.eml" 
Content-Description: Attachment email.eml 
Content-Disposition: attachment; filename="Attachment email.eml"; size=408; 
                creation-date="Mon, 04 Sep 2017 09:59:43 GMT"; 
                modification-date="Mon, 04 Sep 2017 09:59:43 GMT" 
Content-Transfer-Encoding: base64 
 
RnJvbToJQWRtaW5pc3RyYXRvciA8YWRtaW5AdGVuYW50LUVYSEItMTQ3MS5jb20+DQpTZW50OglN 
b25kYXksIFNlcHRlbWJlciA0LCAyMDE3IDM6MjYgUE0NClRvOglTcml2YXJkaGFuIEhlYmJhcg0K 
U3ViamVjdDoJQXR0YWNobWVudCBlbWFpbA0KDQpJIHdpbGwgYXR0YWNoIHRoaXMgZW1haWwgdG8g 
YW5vdGhlciBtYWlsLg0K 
 
--_004_4aade2547798441eab5188a7a2436bc1contoso_-- 
```

## <a name="get-mime-content-of-an-outlook-message-attached-to-an-outlook-item-or-group-post"></a>Получение содержимого MIME сообщения Outlook, вложенного в элемент Outlook или запись в группе

Вы также можете получить представление сообщения Outlook в формате MIME, если сообщение было вложено в [событие](/graph/api/resources/event?view=graph-rest-1.0), [сообщение](/graph/api/resources/message?view=graph-rest-1.0), [задачу](/graph/api/resources/outlooktask?view=graph-rest-beta) или [запись](/graph/api/resources/post?view=graph-rest-1.0) группы Outlook, доступные приложению.

Для этого укажите вложение сообщения и добавьте сегмент `$value` при [получении этого вложения](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment
). Ниже показано несколько распространенных способов получить доступ к вложению. Дополнительные сведения см. в статье [Получение вложения](/graph/api/attachment-get?view=graph-rest-1.0#http-request).

Если сообщение вложено в событие в календаре по умолчанию для пользователя:
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/attachments/{id}/$value
```

Если сообщение вложено в другое событие в почтовом ящике пользователя:
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/messages/{id}/attachments/{id}/$value
```

Если сообщение вложено в задачу Outlook в стандартной папке задач пользователя:
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

Если сообщение вложено в указанную запись группы:
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

### <a name="example"></a>Пример

Ниже приведен пример того, как получить сообщение, вложенное в другое сообщение, где возвращается его текст в формате MIME.

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/messages/AAMkAGUAAA7XW-lAAA=/attachments/AAMkAGUAAA7XW-lAAABEgAQAFBZJBq4EN5FlCSvNV-M-FI=/$value
```

Ниже приведен отклик. Содержимое MIME начинается с заголовка `MIME-Version`. 

<!-- { "blockType": "ignored" } -->
```http
Received: from MWHPR22MB0302.namprd22.prod.outlook.com (2603:10b6:104:5::23)
 by MWHPR2201MB1053.namprd22.prod.outlook.com with HTTPS via
 CO2PR04CA0193.NAMPRD04.PROD.OUTLOOK.COM; Mon, 22 Apr 2019 19:48:20 +0000
Received: from MWHPR22MB1007.namprd22.prod.outlook.com (10.172.167.21) by
 MWHPR22MB0302.namprd22.prod.outlook.com (10.173.53.146) with Microsoft SMTP
 Server (version=TLS1_2, cipher=TLS_ECDHE_RSA_WITH_AES_256_GCM_SHA384) id
 15.20.1813.12; Mon, 22 Apr 2019 19:48:16 +0000
Received: from MWHPR22MB1007.namprd22.prod.outlook.com
 ([fe80::1d05:c2d3:92a:f8dc]) by MWHPR22MB1007.namprd22.prod.outlook.com
 ([fe80::1d05:c2d3:92a:f8dc%9]) with mapi id 15.20.1813.017; Mon, 22 Apr 2019
 19:48:16 +0000
From: Adele Vance <AdeleV@contoso.OnMicrosoft.com>
To: Megan Bowen <MeganB@contoso.OnMicrosoft.com>
Subject: Press conference
Thread-Topic: Press conference
Thread-Index: AQHU+UQNzFWFTilRjECtpiWorLYxqA==
Date: Mon, 22 Apr 2019 19:48:16 +0000
Message-ID:
    <MWHPR22MB100769D1513B3DC0F007B2ECD4220@MWHPR22MB1007.namprd22.prod.outlook.com>
Accept-Language: en-US
Content-Language: en-US
X-MS-Exchange-Organization-AuthAs: Internal
X-MS-Exchange-Organization-AuthMechanism: 04
X-MS-Exchange-Organization-AuthSource: MWHPR22MB1007.namprd22.prod.outlook.com
X-MS-Has-Attach:
X-MS-Exchange-Organization-Network-Message-Id:
    88bed46b-a860-40fb-591e-08d6c75b76c1
X-MS-Exchange-Organization-SCL: -1
X-MS-TNEF-Correlator:
X-MS-Exchange-Organization-RecordReviewCfmType: 0
x-ms-publictraffictype: Email
authentication-results: contoso.OnMicrosoft.com; dkim=none (message not
 signed) header.d=none;contoso.OnMicrosoft.com; dmarc=none action=none
 header.from=contoso.OnMicrosoft.com;
x-originating-ip: [2001:4898:80e8:9:9607:7cf8:4576:961c]
x-ms-office365-filtering-correlation-id: 88bed46b-a860-40fb-591e-08d6c75b76c1
x-microsoft-antispam:
    BCL:0;PCL:0;RULEID:(2390118)(7020095)(4652040)(7021145)(8989299)(4534185)(7022145)(4603075)(4627221)(201702281549075)(8990200)(5600141)(711020)(4605104)(2017052603328)(7177060)(7171020)(7173020)(7193020);SRVR:MWHPR22MB0302;
x-ms-traffictypediagnostic: MWHPR22MB0302:
X-Microsoft-Antispam-Mailbox-Delivery:
    ucf:0;jmr:0;ex:0;auth:0;dest:I;ENG:(750119)(520011016)(706158)(944506303)(944626516);
X-Microsoft-Antispam-Message-Info:
    twccJ5SmB7ZvueSjaTBdmtD3489zlRiHPqiO3DBEil1jBx5xhl/5G/fK2GLgdH0klkE2uoUAAvdvpmxiJezwxCtmn11Nq3kvaOuypDL2TDVdYvWkTfSt4SYfVTp34iBoDlvOEbTh8LTl5J/dz98cgvoRdiE7TUJBXTGvUyVTQX1LG7Xg1hNXMu6XLng6Axdn/ka2NUhmzOa3hEl9yoUI8g3G66Vq3zzVRQFpS+P5+/d1LcbKHsuYMgZNBzBeM6dLnMnwOH9rKXqjV+d72YDnQw4SkbULkoEsQs2Vq0e4URDtkzQwHqcoPv1W2HE4pypmiqkl4M6lJtBccF3MWPP/xNxl6NL5gLSpZCILbg8gQ1UxxX8Kdhd4KWbDa3ayHLHBr11hMNFbGftcUZbZ6jrAtiIGYtGzaAxHqlYC3lUHXZIMdygT76enIJJwklQ1VIp4
Content-Type: multipart/alternative;
    boundary="_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_"
MIME-Version: 1.0

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_
Content-Type: text/plain; charset="iso-8859-1"
Content-Transfer-Encoding: quoted-printable

The press conference will be on May 15. We arranged to have the press gathe=
r at 2pm outside the main entrance.

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_
Content-Type: text/html; charset="iso-8859-1"
Content-Transfer-Encoding: quoted-printable

<html>
<head>
<meta http-equiv=3D"Content-Type" content=3D"text/html; charset=3Diso-8859-=
1">
<style type=3D"text/css" style=3D"display:none;"><!-- P {margin-top:0;margi=
n-bottom:0;} --></style>
</head>
<body dir=3D"ltr">
<div id=3D"divtagdefaultwrapper" style=3D"font-size:12pt;color:#000000;font=
-family:Calibri,Helvetica,sans-serif;" dir=3D"ltr">
<p style=3D"margin-top:0;margin-bottom:0">The press conference will be on M=
ay 15. We arranged to have the press gather at 2pm outside the main entranc=
e.</p>
</div>
</body>
</html>

--_000_MWHPR22MB100769D1513B3DC0F007B2ECD4220MWHPR22MB1007namp_--
```

## <a name="next-steps"></a>Дальнейшие действия

Дополнительные сведения:

- [Получение содержимого MIME вложения](/graph/api/attachment-get?view=graph-rest-1.0#get-the-raw-contents-of-a-file-or-item-attachment) для события, сообщения, задачи Outlook или записи в группе
- [Зачем выполнять интеграцию с почтой Outlook?](outlook-mail-concept-overview.md)
- [Использование API почты](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) и [варианты использования](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) в Microsoft Graph 1.0.
