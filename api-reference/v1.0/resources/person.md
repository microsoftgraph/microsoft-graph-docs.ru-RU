---
title: Тип ресурса person
description: Агрегирование сведений о человеке из почты, контактов и социальных сетей. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога вашей организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype).
author: simonhult
ms.localizationpriority: high
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 33e177875c7e7724659df79d191c2fe07bc1a2a0
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59117804"
---
# <a name="person-resource-type"></a>Тип ресурса person

Пространство имен: microsoft.graph

Агрегирование сведений о человеке из почты, контактов и социальных сетей. В качестве людей могут выступать локальные контакты, контакты из социальных сетей или каталога вашей организации, а также лица, с которыми пользователь недавно общался (например, по почте или в Skype).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
|:---------------|:--------|:----------|
|[List people](../api/user-list-people.md) | **person** |Получение коллекции объектов person, упорядоченных по их релевантности для [пользователя](../resources/user.md).|

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
|:---------------|:--------|:----------|
|birthday|String|День рождения человека.|
|companyName|String|Название компании человека.|
|department|String|Отдел, в котором работает человек.|
|displayName|String|Отображаемое имя человека.|
|scoredEmailAddresses|Коллекция [scoredEmailAddress](scoredemailaddress.md)|Электронные адреса человека.|
|givenName|String|Имя человека.|
|id|String|Уникальный идентификатор человека. Только для чтения.|
|imAddress|String|Адрес SIP VOIP для обмена мгновенными сообщениями для пользователя. Только для чтения.|
|isFavorite|Boolean|Имеет значение `true`, если пользователь добавил этого человека в список избранных.|
|jobTitle|String|Должность человека.|
|officeLocation|String|Расположение офиса человека.|
|personNotes|String|Заметки в произвольной форме о человеке, созданные пользователем.|
|personType|[personType](persontype.md) |Тип человека.|
|phones|Коллекция [phone](phone.md)|Номера телефонов человека.|
|postalAddresses|Коллекция [location](location.md)|Адреса человека.|
|profession|String|Профессия человека.|
|surname|String|Фамилия человека.|
|userPrincipalName|String|Имя участника-пользователя человека. Имя участника-пользователя — это имя для входа, используемое в Интернете и закрепленное за человеком. Оно основано на интернет-стандарте [RFC 822](https://www.ietf.org/rfc/rfc0822.txt). В соответствии с соглашением оно должно быть сопоставлено с именем пользователя для электронной почты. В общем случае оно должно иметь следующий формат: псевдоним@домен.|
|websites|Коллекция [website](website.md)|Веб-сайты человека.|
|yomiCompany|String|Название компании человека, записанное так, как оно звучит по-японски.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "scoredEmailAddresses": [{"@odata.type": "microsoft.graph.scoredEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "imAddress": "string",
  "isFavorite": true,
  "jobTitle": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": {"@odata.type": "microsoft.graph.personType"},
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "surname": "string",
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

