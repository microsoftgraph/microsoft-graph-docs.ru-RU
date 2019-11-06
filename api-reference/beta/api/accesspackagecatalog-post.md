---
title: Создание Акцесспаккажекаталог
description: Создание нового Акцесспаккажекаталог.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9b973310b9cb442f2b95ba4eafd9a2e76ba33fce
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994228"
---
# <a name="create-accesspackagecatalog"></a>Создание Акцесспаккажекаталог

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Создание нового объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) .

## <a name="permissions"></a>Разрешения

Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

| Тип разрешения                        | Разрешения (в порядке повышения привилегий) |
|:---------------------------------------|:--------------------------------------------|
| Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
| Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
| Для приложений                            | Не поддерживается. |

## <a name="http-request"></a>HTTP-запрос

<!-- { "blockType": "ignored" } -->

```http
POST /identityGovernance/entitlementManagement/accessPackageCatalogs
```

## <a name="request-headers"></a>Заголовки запросов

| Имя          | Описание   |
|:--------------|:--------------|
| Authorization | Носитель \{токен\}. Обязательный элемент. |
| Content-Type  | application/json  |

## <a name="request-body"></a>Текст запроса

В тексте запроса добавьте представление объекта [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в формате JSON.  Включите свойства **DisplayName**, **Description**и **исекстерналливисибле** .

## <a name="response"></a>Ответ

В случае успешного выполнения этот метод возвращает код ответа серии 200 и новый объект [акцесспаккажекаталог](../resources/accesspackagecatalog.md) в тексте отклика.

## <a name="examples"></a>Примеры

### <a name="request"></a>Запрос

Ниже приведен пример запроса.

# <a name="httptabhttp"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_accesspackagecatalog_from_accesspackagecatalogs"
}-->

```http
POST https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs
Content-type: application/json

{
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "isExternallyVisible": true
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-accesspackagecatalog-from-accesspackagecatalogs-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-accesspackagecatalog-from-accesspackagecatalogs-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-accesspackagecatalog-from-accesspackagecatalogs-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

Ниже приведен пример отклика.

> **Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
  "displayName": "sales",
  "description": "for employees working with sales and outside sales partners",
  "catalogType": "UserManaged",
  "catalogStatus": "Published",
  "isExternallyVisible": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
