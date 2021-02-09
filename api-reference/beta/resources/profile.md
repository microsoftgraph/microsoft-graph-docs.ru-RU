---
title: Тип ресурса profile
description: Представляет свойства, описательные для пользователя и представленные в общем доступе, интерфейсы пользователей в Microsoft 365 и сторонних службах и интерфейсах через Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 542d5907bd1bc467c32ae58836df04a2c62df36f
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153517"
---
# <a name="profile-resource-type"></a>Тип ресурса profile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства, описательные для пользователя в клиенте, например годовщины и образовательные мероприятия. Эти свойства делиться общими, людей в Microsoft 365 и сторонних служб и опытом через Microsoft Graph. 

Программным образом эти свойства выражаются в виде [связей](#relationships) **ресурса** профиля. Чтобы получить одно из этих свойств навигации или создать экземпляр этих свойств для пользователя, используйте соответствующий метод GET или POST для этого свойства, если это применимо. См. [методы, перечисленные](#methods) ниже.

## <a name="methods"></a>Методы

| Метод                                                                     | Возвращаемый тип                                                    | Описание                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [Получение профиля](../api/profile-get.md)                                       | [profile](profile.md)                                          | Чтение свойств и связей объекта профиля.                                     |
| [Удаление профиля](../api/profile-delete.md)                                 | Нет                                                           | Удаление **объекта** профиля.                                                                 |
| [Создание userAccountInformation](../api/profile-post-accounts.md)           | [userAccountInformation](useraccountinformation.md)            | Создание объекта **userAccountInformation** путем публикации в коллекции учетных записей.        |
| [Список учетных записей](../api/profile-list-accounts.md)                           | [Коллекция userAccountInformation](useraccountinformation.md) | Получить **коллекцию объектов userAccountInformation.**                                          |
| [Создание элементаAddress](../api/profile-post-addresses.md)                     | [itemAddress](itemaddress.md)                                  | Создание нового **элемента itemAddress путем** публикации в коллекции адресов.                         |
| [Адреса списков](../api/profile-list-addresses.md)                         | [Коллекция itemAddress](itemaddress.md)                       | Получить **коллекцию объектов itemAddress.**                                                    |
| [Создание personAnniversary](../api/profile-post-anniversaries.md)           | [personAnniversary](personanniversary.md)                      | Создание нового **personAnniversary** путем публикации в коллекции годовщин.               |
| [Список годовщин](../api/profile-list-anniversaries.md)                 | [Коллекция personAnniversary](personanniversary.md)           | Получить **коллекцию объектов personAnniversary.**                                               |
| [Создание personAward](../api/profile-post-awards.md)                        | [personAward](personaward.md)                                  | Создайте объект **personAward,** опубликовав его в коллекции .                     |
| [Список 1](../api/profile-list-awards.md)                               | [Коллекция personAward](personaward.md)                       | Получить коллекцию **объектов personAward.**                                                     |
| [Создание personCertification](../api/profile-post-certifications.md)        | [personCertification](personcertification.md)                  | Создание объекта **personCertification** путем публикации в коллекции сертификатов.     |
| [Список сертификатов](../api/profile-list-certifications.md)               | [Коллекция personCertification](personcertification.md)       | Получить **коллекцию объектов personCertification.**                                             |
| [Create educationalActivity](../api/profile-post-educationalactivities.md) | [educationalActivity](educationalactivity.md)                  | Создание новой **возможности educationalActivity путем** публикации в коллекции **educationalActivities.** |
| [Список образовательных активов](../api/profile-list-educationalactivities.md) | [коллекция educationalActivity](educationalactivity.md)       | Получить **коллекцию объектов educationalActivity.**                                            |
| [Создание itemEmail](../api/profile-post-emails.md)                          | [itemEmail](itememail.md)                                      | Создание нового **элемента itemEmail путем** публикации в коллекции сообщений электронной почты.                              |
| [Список сообщений электронной почты](../api/profile-list-emails.md)                               | [Коллекция itemEmail](itememail.md)                           | Получить **коллекцию объектов itemEmail.**                                                      |
| [Создание personInterest](../api/profile-post-interests.md)                  | [personInterest](personinterest.md)                            | Создание нового **personInterest путем** публикации в коллекции интересов.                      |
| [Список интересов](../api/profile-list-interests.md)                         | [Коллекция personInterest](personinterest.md)                 | Получить **коллекцию объектов personInterest.**                                                  |
| [Создание languageProficiency](../api/profile-post-languages.md)             | [languageProficiency](languageproficiency.md)                  | Создайте новый **languageProficiency** путем публикации в коллекции языков.                 |
| [Перечисление языков](../api/profile-list-languages.md)                         | [Коллекция languageProficiency](languageproficiency.md)       | Получите **коллекцию объектов languageProficiency.**                                             |
| [Создание personName](../api/profile-post-names.md)                          | [personName](personname.md)                                    | Создание объекта **personName** путем публикации в коллекции имен.                       |
| [Список имен](../api/profile-list-names.md)                                 | [коллекция personName](personname.md)                         | Получить **коллекцию объектов personName.**                                                      |
| [Создание personAnnotation](../api/profile-post-notes.md)                    | [personAnnotation](personannotation.md)                        | Создание объекта **personAnnotation** путем публикации в коллекции заметок.                 |
| [Список заметок](../api/profile-list-notes.md)                                 | [коллекция personAnnotation](personannotation.md)             | Получить **коллекцию объектов personAnnotation.**                                                |
| [Создание itemPatent](../api/profile-post-patents.md)                        | [itemPatent](itempatent.md)                                    | Создание объекта **itemPatent** путем публикации в коллекции патентов.                     |
| [Список патентов](../api/profile-list-patents.md)                             | [Коллекция itemPatent](itempatent.md)                         | Получить **коллекцию объектов itemPatent.**                                                      |
| [Создание itemPhone](../api/profile-post-phones.md)                          | [itemPhone](itemphone.md)                                      | Создание нового itemPhone путем публикации в коллекции телефонов.                                  |
| [Список телефонов](../api/profile-list-phones.md)                               | [Коллекция itemPhone](itemphone.md)                           | Получить **коллекцию объектов itemPhone.**                                                       |
| [Создание workPosition](../api/profile-post-positions.md)                    | [workPosition](workposition.md)                                | Создайте новую позицию, опубликовав ее в коллекции позиций.                            |
| [Позиции списка](../api/profile-list-positions.md)                         | [Коллекция workPosition](workposition.md)                     | Получить **коллекцию объектов workPosition.**                                                    |
| [Создание projectParticipation](../api/profile-post-projects.md)             | [projectParticipation](projectparticipation.md)                | Создание новой **части projectParticipation** путем публикации в коллекции проектов.                 |
| [Список проектов](../api/profile-list-projects.md)                           | [Коллекция projectParticipation](projectparticipation.md)     | Получите **коллекцию объектов projectParticipation.**                                            |
| [Создание itemPublication](../api/profile-post-publications.md)              | [itemPublication](itempublication.md)                          | Создание объекта **itemPublication** путем публикации в коллекции публикаций.           |
| [Список публикаций](../api/profile-list-publications.md)                   | [Коллекция itemPublication](itempublication.md)               | Получить **коллекцию объектов itemPublication.**                                                 |
| [Создание personResponsibility](../api/profile-post-responsibilities.md)     | [personResponsibility](personresponsibility.md)                | Создание объекта **personResponsibility** путем публикации в коллекции обязанностей.  |
| [Список обязанностей](../api/profile-list-responsibilities.md)           | [коллекция personResponsibility](personresponsibility.md)     | Получить **коллекцию объектов personResponsibility.**                                            |
| [Создание skillProficiency](../api/profile-post-skills.md)                   | [skillProficiency](skillproficiency.md)                        | Создайте новую **квалификацию,** опубликовав в коллекции навыков.                       |
| [Список навыков](../api/profile-list-skills.md)                               | [Коллекция skillProficiency](skillproficiency.md)             | Получите **коллекцию объектов skillProficiency.**                                                |
| [Создание webAccount](../api/profile-post-webaccounts.md)                    | [webAccount](webaccount.md)                                    | Создание новой **учетной записи webAccount** путем публикации в коллекции webAccounts.                        |
| [Список webAccounts](../api/profile-list-webaccounts.md)                     | [Коллекция webAccount](webaccount.md)                         | Получить **коллекцию объектов webAccount.**                                                      |
| [Создание personWebsite](../api/profile-post-websites.md)                    | [personWebsite](personwebsite.md)                              | Создание сайта **personWebsite** путем публикации в коллекции веб-сайтов.                        |
| [Список веб-сайтов](../api/profile-list-websites.md)                           | [Коллекция personWebsite](personwebsite.md)                   | Получить **коллекцию объектов personWebsite.**                                                   |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id            |String       | Только для чтения.  |

## <a name="relationships"></a>Связи

| Связь          | Тип                                                         | Описание                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|учетные записи               |[Коллекция userAccountInformation](useraccountinformation.md)| Представляет сведения, специально привязанные к учетной записи пользователя.                                                             |
|addresses              |[Коллекция itemAddress](itemaddress.md)                      | Представляет сведения об адресах, связанных с пользователем.                                                             |
|anniversaries          |[Коллекция personAnniversary](personanniversary.md)          | Представляет сведения о значимых датах, связанных с человеком.                                                                  |
|awards                 |[Коллекция personAward](personaward.md)                      | Представляет сведения о наградах или почетах, связанных с человеком.                                                                  |
|certifications         |[Коллекция personCertification](personcertification.md)      | Представляет сведения о сертификациях, связанных с человеком.                                                                  |
|educationalActivities  |[коллекция educationalActivity](educationalactivity.md)      | Представляет данные, предоставленные пользователем в связи с подложными, учебными, послеунительные или другими образовательными мероприятиями. |
|emails                 |[Коллекция itemEmail](itememail.md)                          | Представляет подробные сведения об адресах электронной почты, связанных с пользователем.                       |
|interests;              |[Коллекция personInterest](personinterest.md)                | Предоставляет подробные сведения об интересах, которые пользователь связал с собой в различных службах.             |
|languages              |[Коллекция languageProficiency](languageproficiency.md)      | Представляет подробные сведения о языках, добавленных пользователем в свой профиль.                                    |
|names                  |[коллекция personName](personname.md)                        | Представляет имена, которые пользователь добавил в свой профиль.                                    |
|notes                  |[коллекция personAnnotation](personannotation.md)            | Представляет заметки, добавленные пользователем в свой профиль.                                    |
|patents                |[Коллекция itemPatent](itempatent.md)                        | Представляет патенты, добавленные пользователем в свой профиль.                                    |
|phones                 |[Коллекция itemPhone](itemphone.md)                          | Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.                            |
|positions              |[Коллекция workPosition](workposition.md)                    | Представляет подробные сведения о должностях, связанных с профилем пользователя.                                    |
|projects               |[Коллекция projectParticipation](projectparticipation.md)    | Представляет подробные сведения о проектах, связанных с пользователем.                                                     |
|publications           |[Коллекция itemPublication](itempublication.md)              | Представляет сведения о любых публикациях, добавленных пользователем в свой профиль.                                                     |
|responsibilities;       |[коллекция personResponsibility](personResponsibility.md)    | Представляет сведения об обязанностях, которые пользователь добавил в свой профиль.                                                     |
|skills.                 |[Коллекция skillProficiency](skillproficiency.md)            | Представляет подробные сведения о навыках, связанных с пользователем в различных службах.                                   |
|webAccounts            |[Коллекция webAccount](webaccount.md)                        | Представляет веб-учетные записи, которые пользователь указал или добавил в свой профиль пользователя.                               |
|websites               |[Коллекция personWebsite](personwebsite.md)                  | Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.                                 |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "keyProperty": "id"
}-->

```json
{
    "id": "String (identifier)"
}
```


