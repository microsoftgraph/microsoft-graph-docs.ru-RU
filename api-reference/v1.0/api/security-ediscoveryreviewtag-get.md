---
title: Получение ediscoveryReviewTag
description: Чтение свойств и связей объекта ediscoveryReviewTag.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 3a4494b3e94cd2ddbd4ab620af5cc5a56a7bb4dd
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839794"
---
# <a name="get-ediscoveryreviewtag"></a>Получение ediscoveryReviewTag
Пространство имен: microsoft.graph.security



Чтение свойств и связей объекта [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) .

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/tags/{ediscoveryReviewTagId}
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files/{ediscoveryFileId}/tags/{ediscoveryReviewTagId}
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files/{ediscoveryFileId}/tags/{ediscoveryReviewTagId}/parent
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/files/{ediscoveryFileId}/tags/{ediscoveryReviewTagId}/childTags/{ediscoveryReviewTagId}
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

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и объект [microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "get_ediscoveryreviewtag"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/tags/062de822f17a4a2e9b833aa3f6c37108
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/tags/$entity",
    "displayName": "My tag",
    "description": null,
    "lastModifiedDateTime": "2022-05-23T19:41:01.7432683Z",
    "childSelectability": "Many",
    "id": "062de822f17a4a2e9b833aa3f6c37108",
    "createdBy": {
        "application": null,
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        }
    }
}
```

