---
title: Тип ресурса messageRule
description: Правило, которое применяется к сообщениям в папке "Входящие" пользователя.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 6147640a221b72716f20bf4a90e74e25a7f9a448
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133765"
---
# <a name="messagerule-resource-type"></a>Тип ресурса messageRule

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Правило, которое применяется к сообщениям в папке "Входящие" пользователя.

В Outlook можно настроить правила для сообщений в папке "Входящие", согласно которым при соблюдении определенных условий выполняются нужные действия. 

Программным способом можно получить доступ к правилам, используя свойство навигации **messageRules** [папки](mailfolder.md) "Входящие". Каждое правило определено ресурсом **messageRule**, доступные действия правил определяются сложным типом [messageRuleActions](messageruleactions.md), а доступные условия и исключения для правил — сложным типом [messageRulePredicates](messagerulepredicates.md).


## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
| actions | [messageRuleActions](messageruleactions.md) | Действия, которые нужно применить к сообщению при выполнении определенных условий. |
| conditions | [messageRulePredicates](messagerulepredicates.md) | Условия, выполнение которых активирует соответствующие действия для указанного правила. |
| displayName | Строка | Отображаемое имя правила. |
| exceptions | [messageRulePredicates](messagerulepredicates.md) | Условия исключения для правила. |
| hasError | Boolean | Указывает, является ли правило ошибкой. Только для чтения. |
| id |Строка|Уникальный идентификатор правила. Только для чтения.|
| isEnabled | Boolean | Указывает, включено ли применение правила к сообщениям. |
| isReadOnly | Boolean | Указывает, доступно ли правило только для чтения и можно ли изменить или удалить его с помощью REST API для правил. |
| sequence | Int32 | Определяет последовательность выполнения правила среди прочих правил. |


## <a name="json-representation"></a>Представление в формате JSON
Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRule"
}-->

```json
{
  "actions": {"@odata.type": "microsoft.graph.messageRuleActions"},
  "conditions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "displayName": "String",
  "exceptions": {"@odata.type": "microsoft.graph.messageRulePredicates"},
  "hasError": "Boolean",
  "id": "String",
  "isEnabled": "Boolean",
  "isReadOnly": "Boolean",
  "sequence": "Int32"
}

```

## <a name="methods"></a>Методы
| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Список правил](../api/mailfolder-list-messagerules.md) | Коллекция [messageRule](messagerule.md) |Получает все объекты **messageRule**, определенные для папки "Входящие" пользователя.|
|[Получение правила](../api/messagerule-get.md) | [messageRule](messagerule.md) |Считывает свойства и отношения объекта **messageRule**.|
|[Создание](../api/mailfolder-post-messagerules.md) | [messageRule](messagerule.md) |Создает объект **messageRule**, определяя набор условий и действий.|
|[Обновление](../api/messagerule-update.md) | [messageRule](messagerule.md) |Изменяет записываемые свойства объекта **messageRule** и сохраняет изменения. |
|[Delete](../api/messagerule-delete.md) | Нет |Удаляет указанный объект **messageRule**. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRule resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


