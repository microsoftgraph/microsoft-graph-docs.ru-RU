---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 297055a6edb4eb4d094406e03b9e4136f1df68c4
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44864107"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>Тип ресурсов openTypeExtension (открытые расширения)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.
Открытые расширения представлены ресурсом **openTypeExtension**. Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).  Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений. Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`. Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.

Пример открытого расширения см. в статье [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).

Открытые расширения поддерживаются указанными ниже ресурсами в соответствующих версиях — общедоступной (1.0 или бета-версии) или предварительной (бета-версии).

| Ресурс | Версия |
|---------------|-------|
| [administrativeUnit](administrativeunit.md)  | Только предварительная версия |
| [event](event.md) для календаря | Общедоступная версия |
| [event](event.md) для календаря группы | Общедоступная версия |
| [post](post.md) цепочки беседы группы | Общедоступная версия |
| [device](device.md) | Общедоступная версия |
| [group](group.md) | Общедоступная версия |
| [message](message.md) | Общедоступная версия |
| [organization](organization.md) | Общедоступная версия |
| [contact](contact.md) (личный контакт) | Общедоступная версия |
| [user](user.md) | Общедоступная версия |

## <a name="outlook-specific-considerations"></a>Специальные рекомендации для Outlook

Каждое открытое расширение, присутствующее в ресурсе Outlook (событии, сообщении или личном контакте), хранится в [именованном свойстве MAPI](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx). Создавая открытые расширения для Outlook, учитывайте, что именованные свойства MAPI в почтовом ящике пользователя — это ограниченный ресурс. Когда будет достигнута квота именованных свойств пользователя, для этого пользователя невозможно будет создавать другие именованные свойства. Это может привести к неожиданным действиям пользователей, для работы которых необходимы именованные свойства.

Руководствуйтесь приведенными ниже рекомендациями при создании открытых расширений в ресурсах Outlook.

- Создайте минимум необходимых расширений. Большинству приложений должно потребоваться не более одного расширения. У расширений нет определенных свойств или структуры, поэтому в одном расширении можно хранить несколько значений.
- Избегайте несогласованного именования расширений (например, на основании вводимых пользователями данных и т. д.). При создании открытого расширения с новым именем, которое ранее не использовалось в почтовом ящике пользователя, всегда создается новое именованное свойство MAPI. При удалении расширения именованное свойство не удаляется.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Использование открытых расширений (для ресурсов Outlook) или расширенных свойств

Открытые расширения — это рекомендуемое решение для большинства сценариев, в которых используется хранение пользовательских данных и доступ к ним. Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md). Вы можете проверить, какие свойства предоставляются с помощью метаданных, на странице [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).

## <a name="json-representation"></a>Представление в формате JSON

Ниже показано представление JSON ресурса.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.openTypeExtension"
}-->

```json
{
  "extensionName": "string",
  "id": "string (identifier)"
}

```

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|extensionName|String|Уникальный текстовый идентификатор для модуля обработки данных открытого типа. Обязательный.|
|id|String| Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.|

## <a name="relationships"></a>Связи

Нет

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md)(в существующем экземпляре ресурса) или новый [контакт](../resources/contact.md), [событие](../resources/event.md)или [сообщение](../resources/message.md) , содержащее объект openTypeExtension. | Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.|
|[Get](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |Чтение свойств и связей объекта openTypeExtension.|
|[Update](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |Обновление объекта openTypeExtension. |
|[Delete](../api/opentypeextension-delete.md) | Нет |Удаление объекта openTypeExtension. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "openTypeExtension resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
