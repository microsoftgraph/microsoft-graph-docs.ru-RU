---
title: Тип ресурса groupLifecyclePolicy
description: Представляет политику жизненного цикла для группы Office 365. Политика жизненного цикла позволяет администраторам устанавливать срок действия групп. Например, срок действия группы истекает через 180 дней. Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени. После продления группа будет оставаться активной в течение определенного политикой количества дней. Например, срок действия группы истекает через 180 дней после продления. Если срок действия группы не продлить, она будет удалена. Группу можно восстановить в течение 30 дней после удаления.
localization_priority: Normal
author: dkershaw10
ms.prod: groups
doc_type: resourcePageType
ms.openlocfilehash: acd1e2b8b66d7cb643e483ee099a3c9909df5d9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532926"
---
# <a name="grouplifecyclepolicy-resource-type"></a>Тип ресурса groupLifecyclePolicy

Пространство имен: microsoft.graph

Представляет политику жизненного цикла для группы Office 365. Политика жизненного цикла позволяет администраторам устанавливать срок действия групп. Например, срок действия группы истекает через 180 дней. Когда срок действия группы истекает, ее владельцы должны продлить его в течение определенного администратором времени. После продления группа будет оставаться активной в течение определенного политикой количества дней. Например, срок действия группы истекает через 180 дней после продления. Если срок действия группы не продлить, она будет удалена. Группу можно восстановить в течение 30 дней после удаления.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Get groupLifecyclePolicy](../api/grouplifecyclepolicy-get.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) |Чтение свойств и связей объекта groupLifecyclePolicy.|
|[Перечисление groupLifecyclePolicies](../api/grouplifecyclepolicy-list.md) | Коллекция [groupLifecyclePolicy](grouplifecyclepolicy.md) | Перечисление всех объектов groupLifecyclePolicy. |
|[Update groupLifecyclePolicy](../api/grouplifecyclepolicy-update.md) | [groupLifecyclePolicy](grouplifecyclepolicy.md) | Обновление объекта groupLifecyclePolicy. |
|[Delete groupLifecyclePolicy](../api/grouplifecyclepolicy-delete.md) | Нет | Удаление объекта groupLifecyclePolicy. |
|[Add a group to a groupLifecyclePolicy](../api/grouplifecyclepolicy-addgroup.md)|Нет| Добавление группы в политику жизненного цикла. |
|[Remove a group from a groupLifecyclePolicy](../api/grouplifecyclepolicy-removegroup.md)|None| Удаление группы из политики жизненного цикла. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|alternateNotificationEmails|Строка| Список адресов электронной почты для отправки уведомлений о группах без владельцев. Можно указать несколько адресов электронной почты, разделив их точкой с запятой. |
|groupLifetimeInDays|Int32| Количество дней до истечения срока действия группы. После продления группа будет оставаться активной в течение указанного количества дней. |
|id|GUID| Уникальный идентификатор политики. Только для чтения.|
|managedGroupTypes|String| Тип группы, к которому применяется политика истечения срока действия. Возможные значения — **All**, **Selected** и **None**. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
}-->

```json
{
  "alternateNotificationEmails": "String",
  "groupLifetimeInDays": 180,
  "id": "Guid (identifier)",
  "managedGroupTypes": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "groupLifecyclePolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
