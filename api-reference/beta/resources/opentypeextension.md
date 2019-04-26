---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открытые расширения (ранее известное как расширения данных Office 365) предоставляют простой способ непосредственного добавления нетипизированных свойств в ресурс в Microsoft Graph.
localization_priority: Normal
author: dkershaw10
ms.openlocfilehash: ba5dbcd6c5ae1705ffe7e89ca6f529280d98adf5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568910"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>Тип ресурсов openTypeExtension (открытые расширения)

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Открытые расширения (ранее известное как расширения данных Office 365) предоставляют простой способ непосредственного добавления нетипизированных свойств в ресурс в Microsoft Graph.
Открытые расширения представлены ресурсом **openTypeExtension**. Все открытые расширения, добавленные в ресурс, отображаются в свойстве навигации **extensions**, которое является производным от абстрактного типа [extension](extension.md).  Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений. Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `Com.Contoso.ContactInfo`. Не указывайте домен Майкрософт (`Com.Microsoft` или `Com.OnMicrosoft`) в имени расширения.

Пример открытого расширения. [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users).

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

## <a name="outlook-specific-considerations"></a>Рекомендации по работе с Outlook

Каждое открытое расширение, присутствующее в ресурсе Outlook (событие, сообщение или личный контакт), хранится в [именованном свойстве MAPI](https://msdn.microsoft.com/library/cc765864(v=office.15).aspx). При создании открытых расширений для Outlook Обратите внимание, что именованные свойства MAPI являются ограниченным ресурсом в почтовом ящике пользователя. Если квота именованного свойства пользователя исчерпана, вы не можете создать дополнительные именованные свойства для этого пользователя. Это может привести к неожиданным последствиям для работы клиентов, использующих именованные свойства.

При создании открытых расширений для ресурсов Outlook придерживайтесь следующих рекомендаций.

- Создайте минимальное необходимое число расширений. Большинству приложений требуется не более одного расширения. Расширения не имеют заданных свойств или структуры, поэтому можно хранить несколько значений в едином расширении.
- Избегайте расширений имен с переменным способом (например, на основе входных данных пользователя и т. д.). Каждый раз при создании открытого расширения с новым именем, которое не использовалось в почтовом ящике пользователя, будет создано новое свойство MAPI named. Удаление расширения не приводит к удалению именованного свойства.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Использование открытых расширений (для ресурсов Outlook) или расширенных свойств

Открытые расширения — это рекомендуемое решение для большинства сценариев, в которых используется хранение пользовательских данных и доступ к ним. Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных API Microsoft Graph](https://developer.microsoft.com/graph/docs/overview/call_api), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md). вы можете проверить, какие свойства предоставляют метаданные на [ https://graph.microsoft.com/v1.0/$metadata](https://graph.microsoft.com/v1.0/$metadata).

## <a name="json-representation"></a>Описание в формате JSON

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

## <a name="relationships"></a>Отношения

Нет

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Post](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) (в существующем экземпляре ресурса) или нового [контакта](../resources/contact.md), [события](../resources/event.md)или [сообщения](../resources/message.md) , содержащего объект openTypeExtension. | Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.|
|[Get](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |Чтение свойств и связей объекта openTypeExtension.|
|[Update](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |Обновление объекта openTypeExtension. |
|[Удаление](../api/opentypeextension-delete.md) | Нет |Удаление объекта openTypeExtension. |

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
