---
title: Тип ресурса Ентитлементманажементсеттингс
description: Представляет параметры на уровне клиента для управления обслуживанием Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f34740bd5e16bb001cd3618edf4c4b669155f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052889"
---
# <a name="entitlementmanagementsettings-resource-type"></a>Тип ресурса Ентитлементманажементсеттингс

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет параметры, управляющие поведением [управления обслуживанием Azure AD](entitlementmanagement-root.md).

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Получение](../api/entitlementmanagementsettings-get.md) | [ентитлементманажементсеттингс](entitlementmanagementsettings.md) | Чтение свойств объекта **ентитлементманажементсеттингс** . |
| [Обновление](../api/entitlementmanagementsettings-update.md) | [ентитлементманажементсеттингс](entitlementmanagementsettings.md) | Обновление свойств объекта **ентитлементманажементсеттингс** . |

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


