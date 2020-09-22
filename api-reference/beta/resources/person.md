---
title: Тип ресурса person
description: Объединение сведений о человеке через почту, контакты и социальные сети. Пользователи могут быть локальными контактами, контактами из социальных сетей, каталогом вашей организации и людьми из недавних коммуникаций (таких как электронная почта и Skype).
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: cc63a75af497a2402955c39a2bcfc8efe370c782
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998056"
---
# <a name="person-resource-type"></a>Тип ресурса person

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Объединение сведений о человеке через почту, контакты и социальные сети. Пользователи могут быть локальными контактами, контактами из социальных сетей, каталогом вашей организации и людьми из недавних коммуникаций (таких как электронная почта и Skype).

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
|displayName|string|Отображаемое имя человека.|
|emailAddresses|Коллекция [ранкедемаиладдресс](rankedemailaddress.md)|Электронные адреса человека.|
|givenName|string|Имя человека.|
|id|string|Уникальный идентификатор человека. Только для чтения.|
|isFavorite|boolean|Имеет значение `true`, если пользователь добавил этого человека в список избранных.|
|mailboxType|string|Тип почтового ящика, представленного адресом электронной почты пользователя.|
|officeLocation;|string|Расположение офиса человека.|
|personNotes|string|Заметки в произвольной форме о человеке, созданные пользователем.|
|personType|string|Тип лица, например список рассылки.|
|phones|Коллекция [phone](phone.md)|Номера телефонов человека.|
|postalAddresses|Коллекция [location](location.md)|Адреса человека.|
|profession|string|Профессия человека.|
|sources|Коллекция [персондатасаурце](persondatasource.md)|Источники, из которых берутся данные пользователя, например, "каталог" или "Контакты Outlook".|
|surname|string|Фамилия человека.|
|title|string|Должность человека.|
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
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


