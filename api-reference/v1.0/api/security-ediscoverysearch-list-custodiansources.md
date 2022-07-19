---
title: Перечисление объектов custodianSource
description: Получение списка источников данных хранения, связанных с поиском eDiscovery.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 02d0f68541578e6c317335665431db2ae5b92886
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66839759"
---
# <a name="list-custodiansources"></a>Перечисление объектов custodianSource
Пространство имен: microsoft.graph.security



Получение списка источников данных хранения, связанных с поиском [eDiscovery](../resources/security-ediscoverysearch.md).

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/custodianSources
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
  "name": "list_datasource"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/custodianSources
```


### <a name="response"></a>Отклик
Ниже приведен пример отклика.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.dataSource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.security.dataSource)",
    "value": [
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/userSources('c25c3914-f9f7-43ee-9cba-a25377e0cec6')",
            "displayName": "MOD Administrator",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "email": "admin@M365x809305.onmicrosoft.com",
            "includedSources": "mailbox,site",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/userSources('43434642-3137-3138-3432-374142313639')",
            "displayName": "Alex Wilber",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "43434642-3137-3138-3432-374142313639",
            "email": "AlexW@M365x809305.OnMicrosoft.com",
            "includedSources": "mailbox,site",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.unifiedGroupSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources('32e14fa4-3106-4bd2-a245-34bf0c718a7e')",
            "displayName": "Design (Mailbox)",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "32e14fa4-3106-4bd2-a245-34bf0c718a7e",
            "includedSources": "mailbox,site",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.siteSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/siteSources('169718e3-a8df-449d-bef4-ee09fe1ddc5d')",
            "displayName": "U.S. Sales",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "169718e3-a8df-449d-bef4-ee09fe1ddc5d",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        },
        {
            "@odata.type": "#microsoft.graph.security.userSource",
            "@odata.id": "https://graph.microsoft.com/v1.0/security/cases/cases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('c25c3914f9f743ee9cbaa25377e0cec6')/userSources('45354430-3730-4232-4236-323230383438')",
            "displayName": "MOD Administrator",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "holdStatus": "0",
            "id": "45354430-3730-4232-4236-323230383438",
            "email": "admin@M365x809305.onmicrosoft.com",
            "includedSources": "mailbox,site",
            "siteWebUrl": null,
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            }
        }
    ]
}
```

