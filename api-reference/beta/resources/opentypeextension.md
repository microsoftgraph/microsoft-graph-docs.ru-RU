---
title: Тип ресурсов openTypeExtension (открытые расширения)
description: Открытые расширения (прежнее название — расширения данных Office 365) позволяют легко добавлять нетипизированные свойства непосредственно в ресурс в Microsoft Graph.
ms.localizationpriority: medium
author: dkershaw10
doc_type: resourcePageType
ms.prod: extensions
ms.openlocfilehash: 57d1af2db82f47be3a3f6faf11768ff2ccf89933
ms.sourcegitcommit: e48fe05125fe1e857225d20ab278352ff7f0911a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2022
ms.locfileid: "66555487"
---
# <a name="opentypeextension-resource-type-open-extensions"></a>Тип ресурсов openTypeExtension (открытые расширения)

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [todo-deprecate-basetaskapi-sharedfeature](../includes/todo-deprecate-basetaskapi-sharedfeature.md)]

Представляет открытые расширения (ранее известные как Office 365 данных), параметр расширяемости, который предоставляет простой [](/graph/extensibility-overview) способ непосредственного добавления нетипизированных свойств к ресурсу в Microsoft Graph.

Любое открытое расширение, добавленное к ресурсу, отображается в **свойстве навигации** расширений. Каждое расширение, помимо пользовательских данных, содержит свойство **extensionName** — единственное предопределенное записываемое свойство для всех расширений. Чтобы обеспечить уникальность имен расширений, можно использовать формат обратных DNS, который зависит от _принадлежащего вам домена_, например `com.contoso.ContactInfo`. **Не используйте домен** Майкрософт (`com.microsoft` или `com.onmicrosoft`) в имени расширения.

Является производным от [абстрактного типа](extension.md) расширения.

Открытые расширения поддерживаются следующими ресурсами.

+ [user](/graph/api/resources/user)
+ [group](/graph/api/resources/group)
<!--+ [administrativeUnit](/graph/api/resources/administrativeunit)-->
+ [contact](/graph/api/resources/contact)
+ [device](/graph/api/resources/device)
+ [событие](/graph/api/resources/event) для календарей пользователей и групп
+ [message](/graph/api/resources/message)
+ [organization](/graph/api/resources/organization)
+ [post](/graph/api/resources/post)
+ [todoTask](todotask.md) 
+ [todoTaskList](todotasklist.md)
+ [baseTaskList](basetasklist.md) (не рекомендуется)
+ [baseTask](basetask.md) (не рекомендуется)

> **Примечание:** \* Из-за существующего ограничения службы делегаты не могут создавать открытые события, добавленные расширением, в общих календарях почтовых ящиков. Попытка сделать это приведет к ответу `ErrorAccessDenied`.

Дополнительные сведения о расширяемости Microsoft Graph, включая ограничения для открытых расширений, см. в [](/graph/extensibility-overview) статье "Добавление настраиваемых свойств к ресурсам с помощью расширений" и "Добавление пользовательских данных пользователям с помощью открытых [расширений"](/graph/extensibility-open-users).

### <a name="outlook-specific-considerations"></a>Специальные рекомендации для Outlook

Каждое открытое расширение, присутствующее в ресурсе Outlook (событии, сообщении или личном контакте), хранится в [именованном свойстве MAPI](/office/client-developer/outlook/mapi/mapi-named-properties). Создавая открытые расширения для Outlook, учитывайте, что именованные свойства MAPI в почтовом ящике пользователя — это ограниченный ресурс. Когда будет достигнута квота именованных свойств пользователя, для этого пользователя невозможно будет создавать другие именованные свойства. Это может привести к неожиданным действиям пользователей, для работы которых необходимы именованные свойства.

Руководствуйтесь приведенными ниже рекомендациями при создании открытых расширений в ресурсах Outlook.

- Создайте минимум необходимых расширений. Большинству приложений должно потребоваться не более одного расширения. У расширений нет определенных свойств или структуры, поэтому в одном расширении можно хранить несколько значений.
- Избегайте несогласованного именования расширений (например, на основании вводимых пользователями данных и т. д.). При создании открытого расширения с новым именем, которое ранее не использовалось в почтовом ящике пользователя, всегда создается новое именованное свойство MAPI. При удалении расширения именованное свойство не удаляется.

### <a name="use-open-extensions-for-outlook-resources-or-extended-properties"></a>Использование открытых расширений (для ресурсов Outlook) или расширенных свойств

Открытые расширения — рекомендуемое решение для большинства сценариев, предполагающее хранение пользовательских данных и доступ к ним. Если вам нужно получить доступ к пользовательским данным для свойств MAPI Outlook, которые еще не предоставлены при помощи [метаданных Microsoft Graph API ](/graph/traverse-the-graph#microsoft-graph-api-metadata), используйте [расширенные свойства и соответствующий REST API](extended-properties-overview.md). Вы можете проверить, какие свойства предоставляются с помощью метаданных в https://graph.microsoft.com/v1.0/$metadata.

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[Создание](../api/opentypeextension-post-opentypeextension.md) | [openTypeExtension](opentypeextension.md) (в существующем экземпляре ресурса) или новый контакт [baseTask](basetask.md), [baseTaskList](basetasklist.md)[,](contact.md) [событие](event.md)[, сообщение](message.md), [запись](post.md), [todoTask](todotask.md) или [todoTaskList](todotasklist.md), содержащий объект openTypeExtension. | Создание объекта openTypeExtension в существующем или новом экземпляре ресурса.|
|[Get](../api/opentypeextension-get.md) | [openTypeExtension](opentypeextension.md) |Чтение свойств и связей объекта openTypeExtension.|
|[Update](../api/opentypeextension-update.md) | [openTypeExtension](opentypeextension.md) |Обновление объекта openTypeExtension. |
|[Delete](../api/opentypeextension-delete.md) | Нет |Удаление объекта openTypeExtension. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|extensionName|String|Уникальный текстовый идентификатор для модуля обработки данных открытого типа. Обязательный.|
|id|String| Полный идентификатор, в котором сцеплены тип расширения и свойство **extensionName**. Только для чтения.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже этот ресурс представлен в формате JSON.

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

## <a name="see-also"></a>См. также

+ [Добавление настраиваемых свойств в ресурсы с помощью расширений](/graph/extensibility-overview)
+ [Добавление пользовательских данных в ресурсы user с помощью открытых расширений](/graph/extensibility-open-users)


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
