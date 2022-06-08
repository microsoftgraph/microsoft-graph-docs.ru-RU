---
title: Создание ediscoverySearch
description: Создайте объект ediscoverySearch.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: b80c3a0dc2d4d43b99abb7ccc4c9e41a8f9b8df5
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2022
ms.locfileid: "65946160"
---
# <a name="create-ediscoverysearch"></a>Создание ediscoverySearch
Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создайте объект [ediscoverySearch](../resources/security-ediscoverysearch.md) .

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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches
```

## <a name="request-headers"></a>Заголовки запросов
|Имя|Описание|
|:---|:---|
|Авторизация|Bearer {token}. Обязательный.|
|Content-Type|application/json. Обязательный.|

## <a name="request-body"></a>Текст запроса
В тексте запроса добавьте представление объекта [ediscoverySearch](../resources/security-ediscoverysearch.md) в формате JSON.

При создании **ediscoverySearch** можно указать следующие свойства.

|Свойство|Тип|Описание|
|:---|:---|:---|
|displayName|String|Отображаемое имя поиска. Обязательный|
|description|Строка|Описание поиска (необязательно).|
|contentQuery|Строка|Строка запроса, используемая для поиска. Строка запроса в формате KQL (язык запросов ключевых слов). Необязательный|
|dataSourceScopes|String|Возможность поиска по всем почтовым ящикам или сайтам в клиенте. Допустимые значения: `none`, `allTenantMailboxes`, `allTenantSites`, `allCaseCustodians`, `allCaseNoncustodialDataSources`. Необязательный параметр.|

## <a name="response"></a>Отклик

В случае успешного выполнения этот метод возвращает код `201 Created` отклика и [объект ediscoverySearch](../resources/security-ediscoverysearch.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
Ниже приведен пример запроса.
<!-- {
  "blockType": "request",
  "name": "create_ediscoverysearch_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches
Content-Type: application/json

{
    "displayName": "My search 2",
    "description": "My first search",
    "contentQuery": "(Author=\"edison\")",
    "custodianSources@odata.bind": [
        "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources/43434642-3137-3138-3432-374142313639",
        "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/siteSources/169718e3-a8df-449d-bef4-ee09fe1ddc5d",
        "https://graph.microsoft.com/beta/security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources('32e14fa4-3106-4bd2-a245-34bf0c718a7e')"
    ],
    "noncustodialSources@odata.bind": [
        "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/35393639323133394345384344303043"
    ]
}
```


### <a name="response"></a>Отклик
Ниже приведен пример ответа.
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.security.ediscoverySearch"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/searches/$entity",
    "dataSourceScopes": "none",
    "description": "My first search",
    "lastModifiedDateTime": "2022-05-23T04:38:07.5787454Z",
    "contentQuery": "(Author=\"edison\")",
    "id": "46867792-68e6-41db-9cd0-f651c2290d91",
    "displayName": "My search 2",
    "createdDateTime": "2022-05-23T04:38:07.5787454Z",
    "lastModifiedBy": null,
    "createdBy": {
        "user": {
            "id": "c25c3914-f9f7-43ee-9cba-a25377e0cec6",
            "displayName": "MOD Administrator",
            "userPrincipalName": "admin@M365x809305.onmicrosoft.com"
        },
        "application": {
            "id": "de8bc8b5-d9f9-48b1-a8ad-b748da725064",
            "displayName": "Graph Explorer"
        }
    }
}
```

