---
title: Перечисление additionalSources
description: Получение списка дополнительных источников, связанных с поиском обнаружения электронных данных.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 812a9500e1c56bc6fa99596499959a5855508a40
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839536"
---
# <a name="list-additionalsources"></a>Перечисление additionalSources
Пространство имен: microsoft.graph.security



Получение списка дополнительных [источников, связанных](../resources/security-datasource.md) с поиском [обнаружения электронных данных](../resources/security-ediscoverysearch.md).

## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения|Разрешения (в порядке повышения привилегий)|
|:---|:---|
|Делегированные (рабочая или учебная учетная запись)|eDiscovery.ReadWrite.All|
|Делегированные (личная учетная запись Майкрософт)|Не поддерживается.|
|Для приложений|Не поддерживается.|

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/additionalSources
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

В случае успешного выполнения `200 OK` этот метод возвращает код отклика и коллекцию объектов [microsoft.graph.security.dataSource](../resources/security-datasource.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "list_ediscoverynoncustodialdatasource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/additionalSources
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.ediscoveryNoncustodialDataSource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches('c61a5860-d634-4d14-aea7-d82b6f4eb7af')/additionalSources",
    "value": [
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "43434642-3137-3138-3432-374142313639",
            "email": "AlexW@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "38423145-4639-4244-4437-464630424139",
            "email": "IrvinS@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "36304536-3033-3845-4639-394538443235",
            "email": "AllanD@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "46454445-3936-3941-4145-463642313642",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "37383041-3143-3731-3744-384643453341",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/sites/",
            "displayName": null,
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "30394337-4541-4632-4532-423832464235",
            "createdBy": {
                "application": null,
                "user": {
                    "id": null,
                    "displayName": null
                }
            }
        }
    ]
}
```

