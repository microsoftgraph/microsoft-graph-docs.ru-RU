---
title: Перечисление файлов ediscoveryFiles
description: Получение списка объектов ediscoveryFile и их свойств.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 9cca478ef643fd799a2dcc34334cf6abe3a43e06
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946395"
---
# <a name="list-ediscoveryfiles"></a>Перечисление файлов ediscoveryFiles
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [ediscoveryFile](../resources/security-ediscoveryfile.md) и их свойств.

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.Read.All, eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files
```

## <a name="optional-query-parameters"></a>Необязательные параметры запросов
Этот метод поддерживает некоторые параметры запросов OData для настройки отклика. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию [объектов ediscoveryFile](../resources/security-ediscoveryfile.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "list_ediscoveryfile"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/files?$top=5
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryFile)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/reviewSets('273f11a1-17aa-419c-981d-ff10d33e420f')/files",
    "@odata.nextLink": "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/files?$top=5&$skiptoken=1",
    "value": [
        {
            "id": "000168cdf05c48d98faac7bff8719726a25da40bb2b9c369fb580b8797abf661",
            "dateTime": "2017-11-02T15:07:10Z",
            "size": 921,
            "name": "Report/CustomVisuals/WordCloud1447959067750/package.json",
            "sourceType": "site",
            "subjectTitle": "Operations Analytics.pbix",
            "extension": "json",
            "mediaType": "application/json; charset=ISO-8859-1",
            "processingStatus": "success",
            "otherProperties": {
                "Source": null,
                "Participants": null,
                "To": null,
                "Cc": null,
                "Bcc": null,
                "Recipients": null,
                "Author": null,
                "CreatedTime": null,
                "Received": null,
                "Sent": null,
                "LastModifiedDate": "2017-11-02T15:07:10Z",
                "MessageType": null,
                "Title": null,
                "EmailHasAttachment": false,
                "EmailImportance": "",
                "WordCount": 25,
                "ErrorIgnored": false,
                "IsFromErrorRemediation": false,
                "EmailSecurity": 0,
                "EmailSensitivity": 0,
                "IsModernAttachment": false,
                "IsEmbeddedDocument": true,
                "ComplianceLabels": null,
                "ConversationId": null,
                "ConversationIndex": null,
                "ItemClass": null,
                "LocationName": null,
                "MeetingStartDate": null,
                "MeetingEndDate": null,
                "ParticipantDomains": null,
                "RecipientDomains": null,
                "Sender": null,
                "SenderDomain": null
            }
        }
    ]
}
```

