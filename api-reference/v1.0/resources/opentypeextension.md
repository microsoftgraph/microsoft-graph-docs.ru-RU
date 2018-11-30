---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открыть extensions (ранее называлась расширения данные Office 365) предоставляют простой способ добавлять нетипизированный свойства непосредственно к ресурсам в Microsoft Graph.
ms.openlocfilehash: eedf61ccdda62ab69673a4489b49db782f514ef0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27025477"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>Тип ресурсов openTypeExtension (открытые расширения)

Открыть extensions (ранее называлась расширения данные Office 365) предоставляют простой способ добавлять нетипизированный свойства непосредственно к ресурсам в Microsoft Graph.

Открытые расширения представлены ресурсом **openTypeExtension**. Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md). Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений.

Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`. Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.

Пример открытого расширения. [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).

Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).

|Ресурс |Версия |
|:---------------|:-------|
| [administrativeUnit](/graph/api/resources/administrativeunit?view=graph-rest-beta)  | Только предварительная версия |
| [event](event.md) для календаря | Общедоступная версия |
| [event](event.md) для календаря группы | Общедоступная версия |
| [post](post.md) цепочки беседы группы | Общедоступная версия |
| [device](device.md) | Общедоступная версия |
| [group](group.md) | Общедоступная версия |
| [message](message.md) | Общедоступная версия |
| [organization](organization.md) | Общедоступная версия |
| [contact](contact.md) (личный контакт) | Общедоступная версия |
| [user](user.md) | Общедоступная версия |

## <a name="outlook-specific-considerations"></a>Вопросы, относящиеся к Outlook

Каждое open расширение на ресурс Outlook (событий, сообщение или личный контакт) хранятся в [MAPI именованное свойство](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx). При создании open расширений для Outlook необходимо учитывайте, что именованные свойства MAPI, ограничение ресурсов в почтовом ящике пользователя. Когда закончится квоту именованное свойство невозможно создать более именованные свойства для этого пользователя. Это может привести к непредсказуемым последствиям от клиентов, зависящие от именованных свойств функции.

При создании open расширений ресурсов Outlook применяются следующие рекомендации:

- Создайте минимальное число необходимых расширений. Большинство приложений требуется не более одного расширения. Расширения не имеют определенный набор свойств или структуры, чтобы можно было хранить несколько значений в одном расширении.
- Избегайте именования расширений в виде переменной (например, на основе введенных данных, и т.д.). Каждый раз, когда open расширение создается новое имя, которое не использовалась в почтовом ящике пользователя перед, будет создан новый MAPI именованное свойство. Удаление расширения не удаляет именованное свойство.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Использование открытия расширения (для ресурсов Outlook) или расширенные свойства

Открыть расширения — это рекомендуемое решение для большинства сценариев с помощью хранение и доступ к пользовательских данных. Если требуется доступ к пользовательские данные для свойства Outlook MAPI, которые еще не предоставляется через [Microsoft Graph API метаданных](https://developer.microsoft.com/graph/docs/overview/call_api), можно использовать [Расширенные свойства и его API -Интерфейс REST](extended-properties-overview.md). Вы можете проверить свойств, которые предоставляет метаданные во [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "baseType": "microsoft.graph.extension",
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>Свойства

|Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|extensionName|String|Уникальный текстовый идентификатор для открытых расширений открытого типа. Обязательно свойство.|
|id|String| Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.|

## <a name="relationships"></a>Связи

Нет

## <a name="methods"></a>Методы

|Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension-post-opentypeextension.md) | Объект [openTypeExtension](opentypeextension.md) (в существующем экземпляре ресурса) либо новый ресурс [contact](../resources/contact.md), [event](../resources/event.md) или [message](../resources/message.md), содержащий объект openTypeExtension. | Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.|
|[Get](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |Чтение свойств и связей объекта openTypeExtension.|
|[Update](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |Обновление объекта openTypeExtension. |
|[Delete](../api/opentypeextension-delete.md) | Нет |Удаление объекта openTypeExtension. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
