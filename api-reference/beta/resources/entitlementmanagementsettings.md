---
title: Тип ресурса Ентитлементманажементсеттингс
description: Представляет параметры на уровне клиента для управления обслуживанием Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b183466b102b480913c3841585ea3349e7ac2386
ms.sourcegitcommit: 0545b031585e605dc3a0fde481015f51f79819c4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/22/2020
ms.locfileid: "45225091"
---
# <a name="entitlementmanagementsettings-resource-type"></a>Тип ресурса Ентитлементманажементсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры, управляющие поведением [управления обслуживанием Azure AD](entitlementmanagement-root.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [получение](../api/entitlementmanagementsettings-get.md); | [ентитлементманажементсеттингс](entitlementmanagementsettings.md) | Чтение свойств объекта **ентитлементманажементсеттингс** . |
| [обновление](../api/entitlementmanagementsettings-update.md). | [ентитлементманажементсеттингс](entitlementmanagementsettings.md) | Обновление свойств объекта **ентитлементманажементсеттингс** . |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|екстерналусерлифециклеактион|Строка|Один из `None` , `BlockSignIn` или `BlockSignInAndDelete` . |
|дайсунтилекстерналусерделетедафтерблоккед|Int64|Если `externalUserLifecycleAction` задано `BlockSignInAndDelete` , то количество дней после блокирования входа от внешнего пользователя до удаления учетной записи.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "baseType": "",
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
