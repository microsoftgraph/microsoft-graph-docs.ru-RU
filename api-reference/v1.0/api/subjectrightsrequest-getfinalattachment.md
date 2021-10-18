---
title: 'subjectRightsRequest: getFinalAttachment'
description: Получите окончательное вложение для запроса на права субъекта.
author: skadam-msft
ms.localizationpriority: medium
ms.prod: compliance
doc_type: apiPageType
ms.openlocfilehash: e619df8cb91510862e067cb1c9468f7d40df0fc6
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/18/2021
ms.locfileid: "60447537"
---
# <a name="subjectrightsrequest-getfinalattachment"></a>subjectRightsRequest: getFinalAttachment
Пространство имен: microsoft.graph

Получите окончательное вложение для запроса на права субъекта. Вложение — это почтовый файл, содержащий все файлы, которые были включены администратором конфиденциальности.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|SubjectRightsRequest.Read.All *, SubjectRightsRequest.ReadWrite.All*|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается|

>[!IMPORTANT]
>Разрешения, отмеченные звездочкой (*), в настоящее время недоступны. Дополнительные сведения см. в статье [Известные проблемы](/graph/known-issues#compliance).

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного сбоя эта функция перенаправит на Microsoft Azure ссылку на хранилище BLOB с маркером SAS и возвращает `302` код ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "subjectRightsRequest_getfinalattachment"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/privacy/subjectRightsRequests/{subjectRightsRequestId}/getFinalAttachment
```


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 302 
```

