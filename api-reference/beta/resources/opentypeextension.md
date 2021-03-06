---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.
localization_priority: Normal
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: de3a4fa33e44788442d0a2ccf1abb4df80e0ea0d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516705"
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
| [administrativeUnit](administrativeunit.md)  | Общедоступная версия |
| [Событие календаря](event.md) | Общедоступная версия |
| [event](event.md) для календаря группы | Общедоступная версия |
| [post](post.md) цепочки беседы группы | Общедоступная версия |
| [Устройство](device.md) | Общедоступная версия |
| [Группа](group.md) | Общедоступная версия |
| [Сообщение](message.md) | Общедоступная версия |
| [Организация](organization.md) | Общедоступная версия |
| [Личный контакт](contact.md) | Общедоступная версия |
| [Пользователь](user.md) | Общедоступная версия |
| [Задача](todotask.md)  | Общедоступная версия |
| [Список задач](todotasklist.md)  | Общедоступная версия |

## <a name="outlook-specific-considerations"></a>Специальные рекомендации для Outlook

Каждое открытое расширение, присутствующее в ресурсе Outlook (событии, сообщении или личном контакте), хранится в [именованном свойстве MAPI](/office/client-developer/outlook/mapi/mapi-named-properties). Создавая открытые расширения для Outlook, учитывайте, что именованные свойства MAPI в почтовом ящике пользователя — это ограниченный ресурс. Когда будет достигнута квота именованных свойств пользователя, для этого пользователя невозможно будет создавать другие именованные свойства. Это может привести к неожиданным действиям пользователей, для работы которых необходимы именованные свойства.

Руководствуйтесь приведенными ниже рекомендациями при создании открытых расширений в ресурсах Outlook.

- Создайте минимум необходимых расширений. Большинству приложений должно потребоваться не более одного расширения. У расширений нет определенных свойств или структуры, поэтому в одном расширении можно хранить несколько значений.
- Избегайте несогласованного именования расширений (например, на основании вводимых пользователями данных и т. д.). При создании открытого расширения с новым именем, которое ранее не использовалось в почтовом ящике пользователя, всегда создается новое именованное свойство MAPI. При удалении расширения именованное свойство не удаляется.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Использование открытых расширений (для ресурсов Outlook) или расширенных свойств

Открытые расширения — рекомендуемое решение для большинства сценариев, предполагающих хранение пользовательских данных и доступ к ним. Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных API Microsoft Graph](../index.md), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md). Вы можете проверить, какие свойства предоставляются с помощью метаданных, на странице [https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).

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
|[Создание](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md)(в существующем экземпляре ресурса) или новый [контакт,](contact.md) [событие,](event.md) [сообщение,](message.md) [сообщение,](post.md) [todoTask](todotask.md)или [todoTaskList,](todotasklist.md) содержащий объект openTypeExtension. | Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.|
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
