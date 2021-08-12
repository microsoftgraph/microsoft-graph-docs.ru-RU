---
title: тип ресурса scopedRoleMembership
description: В членстве с объемной ролью описывается членство пользователя в роли каталога, которая далее передается в административный блок (AU).  Это обеспечивает механизм, позволяющий администратору компании в масштабе клиента делегировать административные привилегии пользователю для управления пользователями и группами в подмножестве организации (подмножество, определяемого АС).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: abhijeetsinha
ms.openlocfilehash: 1a05a741ecc14050d76ca2f414accf13cc3a41f0d80447e521cc74745a1bc3f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54159815"
---
# <a name="scopedrolemembership-resource-type"></a>тип ресурса scopedRoleMembership

Пространство имен: microsoft.graph

В членстве с объемной ролью описывается членство пользователя в роли каталога, которая далее передается в административный блок (AU).  Это обеспечивает механизм, позволяющий администратору всей компании делегировать административные привилегии пользователю для управления пользователями и группами в подмножество организации (подмножество, определяемого АС).

## <a name="methods"></a>Методы
Прямые запросы на этот ресурс не поддерживаются.  В разделе [Административные единицы](administrativeunit.md) см. сведения о том, как запрашивать членство с областью действия ролей, а также добавлять и удалять членство в scoped-role.

## <a name="properties"></a>Свойства
| Свойство   | Тип | Описание |
|:---------------|:--------|:----------|
|administrativeUnitId|Строка|Уникальный идентификатор для административного подразделения, в котором роль каталога|
|id|строка| Уникальный идентификатор для членства в scoped-role. Только для чтения.|
|roleId|Строка| Уникальный идентификатор роли каталога, в котором находится член.|
|roleMemberInfo|[identity](identity.md)| Сведения о удостоверениях членов ролей. Представляет пользователя, который входит в эту область действия.|

## <a name="relationships"></a>Связи
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.scopedRoleMembership"
}-->

```json
{
  "administrativeUnitId": "string",
  "id": "string (identifier)",
  "roleId": "string",
  "roleMemberInfo": {"@odata.type": "microsoft.graph.identity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "scopedRoleMembership resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
