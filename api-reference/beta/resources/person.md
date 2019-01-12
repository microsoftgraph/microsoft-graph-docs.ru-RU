---
title: Тип ресурса person
description: Объединенные данные о сотруднике из всех почты, контакты и социальными сетями. Пользователи могут быть локального контактов, контакты из социальных сетей, вашей организации каталогов и людей из последних коммуникаций (например, электронной почты и Скайп).
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 7f0f3c71769d2ad8927f634b065253cf118316b4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27929384"
---
# <a name="person-resource-type"></a>Тип ресурса person

> **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

Объединенные данные о сотруднике из всех почты, контакты и социальными сетями. Пользователи могут быть локального контактов, контакты из социальных сетей, вашей организации каталогов и людей из последних коммуникаций (например, электронной почты и Скайп).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[List people](../api/user-list-people.md) | **person** |Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|birthday|string|День рождения человека.|
|companyName|string|Название компании человека.|
|department|string|Отдел, в котором работает человек.|
|displayName|строка|Отображаемое имя человека.|
|emailAddresses|[rankedEmailAddress](rankedemailaddress.md) коллекции|Электронные адреса человека.|
|givenName|string|Имя человека.|
|id|строка|Уникальный идентификатор человека. Только для чтения.|
|isFavorite|boolean|Имеет значение `true`, если пользователь добавил этого человека в список избранных.|
|mailboxType|string|Тип почтового ящика, представленного адрес электронной почты пользователя.|
|officeLocation;|string|Расположение офиса человека.|
|personNotes|string|Заметки в произвольной форме о человеке, созданные пользователем.|
|personType|string|Тип лица, например списка рассылки.|
|phones|Коллекция [phone](phone.md)|Номера телефонов человека.|
|postalAddresses|Коллекция [location](location.md)|Адреса человека.|
|profession|string|Профессия человека.|
|sources|[personDataSource](persondatasource.md) коллекции|Источники пользователя данные, поступающие из, например, каталога или контактов Outlook.|
|surname|string|Фамилия человека.|
|должности.|строка|Должность пользователя.|
|userPrincipalName|string|Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.|
|websites|Коллекция [website](website.md)|Веб-сайты человека.|
|yomiCompany|string|Название компании человека, записанное так, как оно звучит по-японски.|

## <a name="relationships"></a>Связи

Нет

## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
