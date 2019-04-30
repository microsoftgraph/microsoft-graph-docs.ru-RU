---
title: Получение содержимого MIME сообщения
description: Multipurpose Internet Mail Extensions (MIME) — это отраслевой стандарт электронной почты. Теперь вы можете использовать сегмент `$value`, чтобы получить содержимое MIME из сообщения Outlook.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: a0b71e3e87a845c995ec2792bab12fc0fc446b59
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32655807"
---
# <a name="get-mime-content-of-a-message-preview"></a><span data-ttu-id="13dd4-104">Получение содержимого MIME сообщения (предварительная версия)</span><span class="sxs-lookup"><span data-stu-id="13dd4-104">Get MIME content of a message (preview)</span></span>

<span data-ttu-id="13dd4-105">MIME — это отраслевой стандарт электронной почты.</span><span class="sxs-lookup"><span data-stu-id="13dd4-105">MIME is an industry email standard.</span></span> <span data-ttu-id="13dd4-106">Многие приложения электронной почты создают сообщения в формате MIME и сохраняют их в файлах с расширением EML.</span><span class="sxs-lookup"><span data-stu-id="13dd4-106">Many email applications create messages in MIME format and save them in files with the .EML extension.</span></span> 

<span data-ttu-id="13dd4-107">Несмотря на то что Outlook _не сохраняет_ сообщения в формате MIME, текст сообщения Outlook в формате MIME можно получить двумя способами:</span><span class="sxs-lookup"><span data-stu-id="13dd4-107">Even though Outlook _does not save_ messages in MIME format, there are two ways you can get an Outlook message body in MIME format:</span></span>

- <span data-ttu-id="13dd4-108">Вы можете добавить сегмент `$value` к операции get-message с этим сообщением.</span><span class="sxs-lookup"><span data-stu-id="13dd4-108">You can append a `$value` segment to a get-message operation on that message.</span></span>
- <span data-ttu-id="13dd4-109">Если сообщение вложено в элемент Outlook или запись в группе, вы можете добавить сегмент `$value` к операции get-attachment с этим элементом или записью в группе.</span><span class="sxs-lookup"><span data-stu-id="13dd4-109">If the message is attached to an Outlook item or group post, you can append a `$value` segment to a get-attachment operation on that item or group post.</span></span>

<span data-ttu-id="13dd4-110">В любом случае приложению должны быть предоставлены [разрешения на доступ](permissions-reference.md#mail-permissions) к элементу Outlook или записи в группе, чтобы применить операцию get-message или get-attachment.</span><span class="sxs-lookup"><span data-stu-id="13dd4-110">In either case, your app must have the appropriate [permissions to access](permissions-reference.md#mail-permissions) the Outlook item or group post in order to apply the get-message or get-attachment operation.</span></span> 

<span data-ttu-id="13dd4-111">Затем вы можете сохранить содержимое текста сообщения в EML-файле и вкладывать файл в записи в бизнес-системах, например для CRM, ERP и отслеживания ошибок.</span><span class="sxs-lookup"><span data-stu-id="13dd4-111">You can then save the message body content in a .EML file and attach the file to records in business systems, such as those for CRM, ERP, and bug tracking.</span></span> 

> <span data-ttu-id="13dd4-112">**Важно!** Возможность получить текст сообщения MIME в настоящее время доступна только в бета-версии.</span><span class="sxs-lookup"><span data-stu-id="13dd4-112">**Important:** The capability to get MIME message body is currently available only in the /beta version.</span></span> <span data-ttu-id="13dd4-113">Как и другие интерфейсы API предварительной версии, она подлежит изменению.</span><span class="sxs-lookup"><span data-stu-id="13dd4-113">Similar to other APIs in preview status, it is subject to change.</span></span> <span data-ttu-id="13dd4-114">Не используйте эту возможность в рабочих приложениях.</span><span class="sxs-lookup"><span data-stu-id="13dd4-114">Do not use this capability in production apps.</span></span> <span data-ttu-id="13dd4-115">Дополнительные сведения см. в статье [Управление версиями и поддержка](versioning-and-support.md).</span><span class="sxs-lookup"><span data-stu-id="13dd4-115">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="what-is-mime"></a><span data-ttu-id="13dd4-116">Что такое MIME?</span><span class="sxs-lookup"><span data-stu-id="13dd4-116">What is MIME?</span></span>

<span data-ttu-id="13dd4-117">MIME — это стандарт, используемый для электронной почты в Интернете, чтобы передавать контент следующих типов по протоколу SMTP:</span><span class="sxs-lookup"><span data-stu-id="13dd4-117">MIME is a standard used by internet email to transmit the following types of content via SMTP:</span></span> 

- <span data-ttu-id="13dd4-118">сообщение в формате обычного текста;</span><span class="sxs-lookup"><span data-stu-id="13dd4-118">plain text message</span></span>
- <span data-ttu-id="13dd4-119">сообщение с альтернативным содержимым (т. е. с обычным текстом и HTML);</span><span class="sxs-lookup"><span data-stu-id="13dd4-119">Message with alternative content (i.e., in both plain text and HTML)</span></span>
- <span data-ttu-id="13dd4-120">ответ, в который вложено исходное сообщение;</span><span class="sxs-lookup"><span data-stu-id="13dd4-120">Reply message with the original message attached</span></span>
- <span data-ttu-id="13dd4-121">текстовое сообщение с вложенными изображениями, звуковыми файлами, видео или файлами приложений;</span><span class="sxs-lookup"><span data-stu-id="13dd4-121">Text message with attachments of image, audio, video, or application files</span></span>  
- <span data-ttu-id="13dd4-122">другие конструкции сообщений.</span><span class="sxs-lookup"><span data-stu-id="13dd4-122">Other message constructs</span></span>

<span data-ttu-id="13dd4-123">Ниже представлены типичные заголовки MIME в сообщении.</span><span class="sxs-lookup"><span data-stu-id="13dd4-123">The following are typical MIME headers in a message.</span></span> <span data-ttu-id="13dd4-124">Дополнительные сведения см. в статье [RFC 2045](https://tools.ietf.org/html/rfc2045).</span><span class="sxs-lookup"><span data-stu-id="13dd4-124">For more information, see [RFC 2045](https://tools.ietf.org/html/rfc2045).</span></span>

- <span data-ttu-id="13dd4-125">`MIME-Version` — указывает, что сообщение представлено в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="13dd4-125">`MIME-Version` - Indicates the message is MIME-formatted.</span></span>
- <span data-ttu-id="13dd4-126">`Content-Type` — указывает тип мультимедиа сообщения или его части, представленный свойствами *type* и *subtype*.</span><span class="sxs-lookup"><span data-stu-id="13dd4-126">`Content-Type` - Indicates the media type of the message or a part of the message, represented by a *type* and *subtype*.</span></span> <span data-ttu-id="13dd4-127">Он также включает поле `boundary`, указывающее строку в виде границы MIME или границы инкапсуляции (в зависимости от расположения `Content-Type`).</span><span class="sxs-lookup"><span data-stu-id="13dd4-127">It also includes a `boundary` field which specifies a string as the MIME boundary or as the encapsulation boundary, depending on the location of `Content-Type`.</span></span> 
- <span data-ttu-id="13dd4-128">`Content-Disposition` — предоставляет сведения о вложении, например стиль его презентации (`inline` или `attachment`), имена файлов, а также даты создания и последнего изменения.</span><span class="sxs-lookup"><span data-stu-id="13dd4-128">`Content-Disposition` - Provides details of an attachment such as its presentation style (`inline` or `attachment`), filenames, and creation and last modification dates.</span></span>
- <span data-ttu-id="13dd4-129">`Content-Transfer-Encoding` — указывает метод шифрования, используемый для представления двоичных данных.</span><span class="sxs-lookup"><span data-stu-id="13dd4-129">`Content-Transfer-Encoding` - Specifies the encoding method to represent binary data.</span></span>

## <a name="get-mime-content-of-an-outlook-message"></a><span data-ttu-id="13dd4-130">Получение содержимого MIME сообщения Outlook</span><span class="sxs-lookup"><span data-stu-id="13dd4-130">Get MIME content of an Outlook message</span></span>

<span data-ttu-id="13dd4-131">Вы можете получить представление сообщения в формате MIME, добавление сегмента `$value` при [получении сообщения](/graph/api/message-get?view=graph-rest-beta):</span><span class="sxs-lookup"><span data-stu-id="13dd4-131">You can get the MIME representation of a message by appending the `$value` segment when [getting the message](/graph/api/message-get?view=graph-rest-beta):</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/messages/{id}/$value
```

### <a name="example"></a><span data-ttu-id="13dd4-132">Пример</span><span class="sxs-lookup"><span data-stu-id="13dd4-132">Example</span></span>

<span data-ttu-id="13dd4-133">Ниже приведен пример, в котором запрашивается возврат сообщения из почтового ящика вошедшего пользователя вместе с его содержимым в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="13dd4-133">The following is an example that requests a message in the signed-in user's mailbox to be returned with its MIME content.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/messages/4aade2547798441eab5188a7a2436bc1/$value
```

<span data-ttu-id="13dd4-134">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="13dd4-134">The following is an example of the response.</span></span> <span data-ttu-id="13dd4-135">Содержимое MIME начинается с заголовка `MIME-Version`.</span><span class="sxs-lookup"><span data-stu-id="13dd4-135">The MIME content begins with the `MIME-Version` header.</span></span> 

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

## <a name="get-mime-content-of-an-outlook-message-attached-to-an-outlook-item-or-group-post"></a><span data-ttu-id="13dd4-136">Получение содержимого MIME сообщения Outlook, вложенного в элемент Outlook или запись в группе</span><span class="sxs-lookup"><span data-stu-id="13dd4-136">Get MIME content of an Outlook message attached to an Outlook item or group post</span></span>

<span data-ttu-id="13dd4-137">Вы также можете получить представление сообщения Outlook в формате MIME, если сообщение было вложено в [событие](/graph/api/resources/event?view=graph-rest-beta), [сообщение](/graph/api/resources/message?view=graph-rest-beta), [задачу](/graph/api/resources/outlooktask?view=graph-rest-beta) или [запись](/graph/api/resources/post?view=graph-rest-beta) группы Outlook, доступной приложению.</span><span class="sxs-lookup"><span data-stu-id="13dd4-137">You can also get the MIME representation of an Outlook message, if the message has been attached to an Outlook [event](/graph/api/resources/event?view=graph-rest-beta), [message](/graph/api/resources/message?view=graph-rest-beta), [task](/graph/api/resources/outlooktask?view=graph-rest-beta), or group [post](/graph/api/resources/post?view=graph-rest-beta) that your app can access.</span></span>

<span data-ttu-id="13dd4-138">Для этого укажите вложение сообщения и добавьте сегмент `$value` при [получении этого вложения](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment
).</span><span class="sxs-lookup"><span data-stu-id="13dd4-138">To do that, identify the message attachment, and append the `$value` segment when [getting that attachment](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment
).</span></span> <span data-ttu-id="13dd4-139">Ниже показано несколько распространенных способов получить доступ к вложению.</span><span class="sxs-lookup"><span data-stu-id="13dd4-139">The following shows a few common ways to access an attachment.</span></span> <span data-ttu-id="13dd4-140">Дополнительные сведения см. в статье [Получение вложения](/graph/api/attachment-get?view=graph-rest-beta#http-request).</span><span class="sxs-lookup"><span data-stu-id="13dd4-140">See [get attachment](/graph/api/attachment-get?view=graph-rest-beta#http-request) for more information.</span></span>

<span data-ttu-id="13dd4-141">Если сообщение вложено в событие в календаре по умолчанию для пользователя:</span><span class="sxs-lookup"><span data-stu-id="13dd4-141">If the message is attached to an event in the user's default calendar:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/events/{id}/attachments/{id}/$value
```

<span data-ttu-id="13dd4-142">Если сообщение вложено в другое событие в почтовом ящике пользователя:</span><span class="sxs-lookup"><span data-stu-id="13dd4-142">If the message is attached to another message in the user's mailbox:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/messages/{id}/attachments/{id}/$value
```

<span data-ttu-id="13dd4-143">Если сообщение вложено в задачу Outlook в стандартной папке задач пользователя:</span><span class="sxs-lookup"><span data-stu-id="13dd4-143">If the message is attached to an Outlook task in the user's default task folder:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id}/outlook/tasks/{id}/attachments/{id}/$value
```

<span data-ttu-id="13dd4-144">Если сообщение вложено в указанную запись группы:</span><span class="sxs-lookup"><span data-stu-id="13dd4-144">If the message is attached to the specified group post:</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/threads/{id}/posts/{id}/attachments/{id}/$value
```

### <a name="example"></a><span data-ttu-id="13dd4-145">Пример</span><span class="sxs-lookup"><span data-stu-id="13dd4-145">Example</span></span>

<span data-ttu-id="13dd4-146">Ниже приведен пример того, как получить сообщение, вложенное в другое сообщение, где возвращается его текст в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="13dd4-146">The following is an example that gets a message that has been attached to another message, and returns the body in MIME format.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/me/messages/AAMkAGUAAA7XW-lAAA=/attachments/AAMkAGUAAA7XW-lAAABEgAQAFBZJBq4EN5FlCSvNV-M-FI=/$value
```

<span data-ttu-id="13dd4-147">Ниже приведен отклик.</span><span class="sxs-lookup"><span data-stu-id="13dd4-147">The following is an example of the response.</span></span> <span data-ttu-id="13dd4-148">Содержимое MIME начинается с заголовка `MIME-Version`.</span><span class="sxs-lookup"><span data-stu-id="13dd4-148">The MIME content begins with the `MIME-Version` header.</span></span> 

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

## <a name="next-steps"></a><span data-ttu-id="13dd4-149">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="13dd4-149">Next steps</span></span>

<span data-ttu-id="13dd4-150">Дополнительные сведения:</span><span class="sxs-lookup"><span data-stu-id="13dd4-150">Find out more about:</span></span>

- <span data-ttu-id="13dd4-151">[Получение содержимого MIME вложения](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment) для события, сообщения, задачи Outlook или записи в группе</span><span class="sxs-lookup"><span data-stu-id="13dd4-151">[Get the MIME content of an item attachment](/graph/api/attachment-get?view=graph-rest-beta#get-the-raw-contents-of-a-file-or-item-attachment) to an event, message, Outlook task, or group post</span></span>
- [<span data-ttu-id="13dd4-152">Зачем выполнять интеграцию с почтой Outlook?</span><span class="sxs-lookup"><span data-stu-id="13dd4-152">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="13dd4-153">[Использование API почты](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) и [варианты использования](/graph/api/resources/mail-api-overview?view=graph-rest-beta#common-use-cases) в бета-версии Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="13dd4-153">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-beta#common-use-cases) in Microsoft Graph v1.0.</span></span>
