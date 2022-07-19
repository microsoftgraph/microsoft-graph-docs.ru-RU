---
title: Перечисление запросов
description: Получение списка запросов, связанных с набором проверки обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 78b891082e0ec4e6c920346bcedfb65585d9216f
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839524"
---
# <a name="list-queries"></a>Перечисление запросов
Пространство имен: microsoft.graph.security



Получение списка запросов [, связанных](../resources/security-ediscoveryreviewsetquery.md) с набором проверки обнаружения электронных данных.

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/reviewSets/{ediscoveryReviewSetId}/queries
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

В случае успешного `200 OK` выполнения этот метод возвращает код отклика и коллекцию объектов [microsoft.graph.security.ediscoveryReviewSetQuery](../resources/security-ediscoveryreviewsetquery.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "list_ediscoveryreviewsetquery"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/58399dff-cebe-478f-b1af-d3227f1fd645/reviewSets/273f11a1-17aa-419c-981d-ff10d33e420f/queries
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryReviewSetQuery)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('58399dff-cebe-478f-b1af-d3227f1fd645')/reviewSets('273f11a1-17aa-419c-981d-ff10d33e420f')/queries",
    "value": [
        {
            "lastModifiedDateTime": "2022-05-29T20:49:47.9289317Z",
            "contentQuery": "((((FileClass=\"Email\") AND (InclusiveType=\"InclusiveMinus\" OR InclusiveType=\"Inclusive\")) OR ((FileClass=\"Attachment\") AND (UniqueInEmailSet=\"true\")) OR ((FileClass=\"Document\") AND (MarkAsRepresentative=\"Unique\")) OR ((FileClass=\"Conversation\"))))",
            "id": "837335b0-1943-444d-a3d1-5522cc21c5a4",
            "displayName": "[AutoGen] For Review",
            "createdDateTime": "2022-05-29T20:49:47.9289317Z",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        },
        {
            "lastModifiedDateTime": "2022-05-29T20:49:48.0539099Z",
            "contentQuery": "((FileType:gz OR FileType:gzip OR FileType:bz2 OR FileType:zip OR FileType:7z OR FileType:rar OR FileType:vhd OR FileType:mbox OR FileType:pst OR FileType:sfx) OR (Size<\"3072B\" AND (FileType:gif OR FileType:bmp OR FileType:png OR FileType:jpg OR FileType:jpeg OR FileType:tif OR FileType:tiff OR FileType:emf OR FileType:pct OR FileType:pic)))",
            "id": "977ad4d5-3e5c-4594-8cb6-7d09dbcddf21",
            "displayName": "[AutoGen] Potentially Immaterial Items",
            "createdDateTime": "2022-05-29T20:49:48.0539099Z",
            "createdBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            },
            "lastModifiedBy": {
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": "MOD Administrator",
                    "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
                }
            }
        }
    ]
}
```

