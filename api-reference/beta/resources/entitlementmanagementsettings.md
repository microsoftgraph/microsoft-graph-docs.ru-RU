---
title: тип ресурса entitlementManagementSettings
description: Представляет параметры для управления правами Azure AD для всех клиентов.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 1b6138bc52e5686af94a94cfa13762b71a6242c4
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945692"
---
# <a name="entitlementmanagementsettings-resource-type"></a>тип ресурса entitlementManagementSettings

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры, которые контролируют поведение управления правами [Azure AD.](entitlementmanagement-root.md)

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/entitlementmanagementsettings-get.md); | [entitlementManagementSettings](entitlementmanagementsettings.md) | Ознакомьтесь с свойствами объекта **entitlementManagementSettings.** |
| [Обновление](../api/entitlementmanagementsettings-update.md) | [entitlementManagementSettings](entitlementmanagementsettings.md) | Обновление свойств объекта **entitlementManagementSettings.** |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|externalUserLifecycleAction|Строка|Один `None` из `BlockSignIn` , или `BlockSignInAndDelete` . |
|daysUntilExternalUserDeletedAfterBlocked|Int64|Если **externalUserLifecycleAction** — количество дней после блокировки внешнего пользователя до удаления `BlockSignInAndDelete` учетной записи.|

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


