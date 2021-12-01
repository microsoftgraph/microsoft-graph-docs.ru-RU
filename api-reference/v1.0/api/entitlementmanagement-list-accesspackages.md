---
title: Пакеты доступа к спискам
description: Извлечение списка объектов accessPackage.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 11e21b61322507e7791837fc52557d4854c645e9
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242938"
---
# <a name="list-accesspackages"></a>Пакеты доступа к спискам

Пространство имен: microsoft.graph


Извлечение списка [объектов accessPackage.](../resources/accesspackage.md)  В итоговом списке содержатся все пакеты доступа, которые вызывающий имеет доступ к считыву, во всех каталогах.

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
GET /identityGovernance/entitlementManagement/accessPackages
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса

Этот метод поддерживает параметры `$select` `$filter` запроса oData и OData для настройки ответа. Например, чтобы получить политики пакета доступа для каждого пакета доступа, добавьте `$expand=accessPackageAssignmentPolicies` . Чтобы найти пакеты доступа с определенным именем, включайте фильтр, `$filter=contains(tolower(displayName),'team')` например, в запрос. Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).

## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов accessPackage](../resources/accesspackage.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "list_accesspackage"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.accessPackage)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.accessPackage",
      "id": "114d3459-3459-114d-5934-4d1159344d11",
      "displayName": "Access package for testing",
      "description": "Sample access package",
      "isHidden": false,
      "createdDateTime": "2019-01-27T18:19:50.74Z",
      "modifiedDateTime": "2019-01-27T18:19:50.74Z"
    }
  ]
}
```


