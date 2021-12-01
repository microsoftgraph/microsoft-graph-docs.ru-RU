---
title: Получить accessPackage
description: Извлечение свойств и связей объекта accessPackage.
author: markwahl-msft
ms.localizationpriority: medium
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: bb983bf7d471530a3fa7ec3fd61da31a5d7e9c5b
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/01/2021
ms.locfileid: "61242806"
---
# <a name="get-accesspackage"></a>Получить accessPackage

Пространство имен: microsoft.graph


Извлечение свойств и связей объекта [accessPackage.](../resources/accesspackage.md)

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
GET /identityGovernance/entitlementManagement/accessPackages/{accessPackageId}
```

## <a name="optional-query-parameters"></a>Необязательные параметры запроса

Этот метод поддерживает параметр `$select` [запроса OData для](/graph/query-parameters) получения определенных свойств.



## <a name="request-headers"></a>Заголовки запросов

| Имя      |Описание|
|:----------|:----------|
| Авторизация | Носитель \{токен\}. Обязательный. |

## <a name="request-body"></a>Текст запроса
Не указывайте текст запроса для этого метода.

## <a name="response"></a>Отклик

В случае успешной работы этот метод возвращает код отклика и запрашиваемого объекта `200 OK` [accessPackage](../resources/accesspackage.md) в тексте ответа.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityGovernance/entitlementManagement/accessPackages/114d3459-3459-114d-5934-4d1159344d11
```


### <a name="response"></a>Отклик
>**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "114d3459-3459-114d-5934-4d1159344d11",
  "displayName": "Access package for testing",
  "description": "Sample access package",
  "isHidden": false,
  "createdDateTime": "2019-01-27T18:19:50.74Z",
  "modifiedDateTime": "2019-01-27T18:19:50.74Z"
}
```

