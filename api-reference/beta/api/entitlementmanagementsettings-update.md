---
title: Обновление entitlementManagementSettings
description: Обновление объекта entitlementManagementSettings, чтобы изменить одно или несколько его свойств.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: f1b95cf9fdeb38d998fcd153d36611e5e0d43328
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787016"
---
# <a name="update-entitlementmanagementsettings"></a>Обновление entitlementManagementSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Обновим [существующий объект entitlementManagementSettings,](../resources/entitlementmanagementsettings.md) чтобы изменить одно или несколько его свойств.


## <a name="permissions"></a>Разрешения
Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).

|Тип разрешения                        | Разрешения (в порядке повышения привилегий)              |
|:--------------------------------------|:---------------------------------------------------------|
|Делегированные (рабочая или учебная учетная запись)     | EntitlementManagement.ReadWrite.All |
|Делегированные (личная учетная запись Майкрософт) | Не поддерживается. |
|Приложение                            | EntitlementManagement.ReadWrite.All |

## <a name="http-request"></a>HTTP-запрос
<!-- { "blockType": "ignored" } -->
```http
PATCH /identityGovernance/entitlementManagement/settings
```
## <a name="request-headers"></a>Заголовки запросов
| Имя         | Описание |
|:-------------|:------------|
| Авторизация | Носитель \{токен\}. Обязательный. |
| Content-Type  | application/json. Обязательный. |

## <a name="request-body"></a>Текст запроса
В теле запроса поставляем представление JSON параметров объекта [entitlementManagementSettings.](../resources/entitlementmanagementsettings.md)

## <a name="response"></a>Отклик
В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.

## <a name="example"></a>Пример

### <a name="request"></a>Запрос


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_entitlementManagementSettings"
}-->
```http
PATCH https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/settings
Content-type: application/json

{
  "externalUserLifecycleAction": "None"
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-entitlementmanagementsettings-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-entitlementmanagementsettings-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-entitlementmanagementsettings-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-entitlementmanagementsettings-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Отклик

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!--
{
  "type": "#page.annotation",
  "description": "Update entitlementManagementSettings",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


