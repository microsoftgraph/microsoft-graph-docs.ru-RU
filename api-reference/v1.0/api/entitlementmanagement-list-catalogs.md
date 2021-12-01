---
title: Список accessPackageCatalogs
description: Извлечение списка объектов accessPackageCatalog.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 67547de703081633ff953f0baffe0cfcc40d94aa
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242847"
---
# <a name="list-catalogs"></a>Каталоги списков

Пространство имен: microsoft.graph

Извлечение списка [объектов accessPackageCatalog.](../resources/accesspackagecatalog.md)

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityGovernance/entitlementManagement/catalogs
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса

Этот метод поддерживает параметры `$select` `$filter` запроса OData и OData для настройки `$expand` ответа. Например, чтобы получить пакеты доступа в каждом каталоге, включайте `$expand=accessPackages` в запрос. Чтобы найти каталоги пакетов доступа с определенным именем, включайте фильтр, `$filter=contains(tolower(displayName),'staff')` например, в запрос. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [accessPackageCatalog](../resources/accesspackagecatalog.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_accesspackagecatalog"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/catalogs
```

### <a name="response"></a>Отклик

>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackageCatalog)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1bf99ed-99ed-b1bf-ed99-bfb1ed99bfb1",
      "displayName": "Access package catalog for testing",
      "description": "Sample access package catalog",
      "catalogType": "userManaged",
      "state": "published",
      "isExternallyVisible": false,
      "createdDateTime": "2019-01-27T18:19:50.74Z",
      "modifiedDateTime": "2019-01-27T18:19:50.74Z"
    }
  ]
}
```



