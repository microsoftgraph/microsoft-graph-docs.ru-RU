---
title: Перечисление объектов unifiedGroupSources хранителя
description: Получение списка объектов unifiedGroupSource хранителя и их свойств.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 6c3c36a1958196844db3d97bc0d7b45740915727
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946311"
---
# <a name="list-custodians-unifiedgroupsources"></a>Перечисление объектов unifiedGroupSources хранителя
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Получение списка объектов [unifiedGroupSource](../resources/security-unifiedgroupsource.md) и их свойств.

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
GET /security/cases/ediscoveryCases/{ediscoveryCaseId}/custodians/{custodianId}/unifiedGroupSources
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

В случае успешного выполнения этот метод возвращает код `200 OK` отклика и коллекцию объектов [unifiedGroupSource](../resources/security-unifiedgroupsource.md) в теле отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "list_unifiedgroupsource"
}
-->
``` http
GET https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/unifiedGroupSources
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.security.unifiedGroupSource)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources",
    "value": [
        {
            "@odata.id": "https://graph.microsoft.com/v1.0/groups/32e14fa4-3106-4bd2-a245-34bf0c718a7e",
            "displayName": "Design (Mailbox)",
            "createdDateTime": "2022-05-23T02:35:42.926309Z",
            "holdStatus": "applied",
            "id": "32e14fa4-3106-4bd2-a245-34bf0c718a7e",
            "includedSources": "mailbox,site",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            },
            "group": {
                "email": "Design@M365x809305.onmicrosoft.com",
                "webUrl": "https://m365x809305.sharepoint.com/sites/Design",
                "id": "32e14fa4-3106-4bd2-a245-34bf0c718a7e",
                "displayName": "Design (Mailbox)",
                "createdDateTime": "2022-05-23T02:35:42.926309Z"
            }
        },
        {
            "@odata.id": "https://graph.microsoft.com/v1.0/groups/21be9868-b58b-4f8b-800c-591e9ad8d4ec",
            "displayName": "CEO Connection (Mailbox)",
            "createdDateTime": "2022-05-23T02:35:42.926309Z",
            "holdStatus": "applied",
            "id": "21be9868-b58b-4f8b-800c-591e9ad8d4ec",
            "includedSources": "mailbox,site",
            "createdBy": {
                "application": null,
                "user": {
                    "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
                    "displayName": null
                }
            },
            "group": {
                "email": "ceoconnection@M365x809305.onmicrosoft.com",
                "webUrl": "https://m365x809305.sharepoint.com/sites/ceoconnection",
                "id": "21be9868-b58b-4f8b-800c-591e9ad8d4ec",
                "displayName": "CEO Connection (Mailbox)",
                "createdDateTime": "2022-05-23T02:35:42.926309Z"
            }
        }
    ]
}
```

