---
title: Тип ресурса entitlementManagementSettings
description: Представляет параметры для всего клиента для управления правами Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d5cc340837f173924802196bf12c9a63f26949a
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50159124"
---
# <a name="entitlementmanagementsettings-resource-type"></a>Тип ресурса entitlementManagementSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры, управляющие поведением управления [правами Azure AD.](entitlementmanagement-root.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение](../api/entitlementmanagementsettings-get.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Чтение свойств объекта **entitlementManagementSettings.** |
| [Обновление](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Обновление свойств объекта **entitlementManagementSettings.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|externalUserLifecycleAction|String|Один из `None` `BlockSignIn` , или `BlockSignInAndDelete` . |
|daysUntilExternalUserDeletedAfterBlocked|Int64|Если это так, то количество дней после блокировки внешнего пользователя на вход до удаления его `externalUserLifecycleAction` `BlockSignInAndDelete` учетной записи.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "keyProperty": ""
}-->

```json
{
  "externalUserLifecycleAction": "String",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entitlementManagementSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


