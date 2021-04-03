---
title: Тип ресурса профиля
description: Представляет свойства, которые являются описательными для пользователя и которые всплыли в общих, люди испытывают в Microsoft 365 и сторонних служб и опытом с помощью Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: ca71d7a559fa6549e676c5e2851711889ac23e8a
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/02/2021
ms.locfileid: "51509326"
---
# <a name="profile-resource-type"></a>Тип ресурса профиля

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства, описательные для пользователя в клиенте, например, юбилеи и образовательные мероприятия. Эти свойства всплыли в общих, люди опытом в Microsoft 365 и сторонних служб и опытом с помощью Microsoft Graph. 

Программным образом эти свойства выражены как [связи](#relationships) ресурса **профиля.** Чтобы получить одно из этих свойств навигации или создать экземпляр этих свойств для пользователя, используйте соответствующий метод GET или POST в этом свойстве, где это применимо. Ниже приведены [методы.](#methods)

## <a name="methods"></a>Методы

| Метод                                                                     | Возвращаемый тип                                                    | Описание                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [Получение профиля](../api/profile-get.md)                                       | [profile](profile.md)                                          | Чтение свойств и связей объекта профиля.                                     |
| [Удаление профиля](../api/profile-delete.md)                                 | Нет                                                           | Удаление **объекта профиля.**                                                                 |
| [Создание userAccountInformation](../api/profile-post-accounts.md)           | [userAccountInformation](useraccountinformation.md)            | Создайте новый **объект userAccountInformation,** разместив в коллекции учетных записей.        |
| [Учетные записи списка](../api/profile-list-accounts.md)                           | [коллекция userAccountInformation](useraccountinformation.md) | Получите **коллекцию объектов userAccountInformation.**                                          |
| [Создание itemAddress](../api/profile-post-addresses.md)                     | [itemAddress](itemaddress.md)                                  | Создайте новый **itemAddress,** разместив в коллекции адресов.                         |
| [Адреса списков](../api/profile-list-addresses.md)                         | [коллекция itemAddress](itemaddress.md)                       | Получите **коллекцию объектов itemAddress.**                                                    |
| [Создание personAnniversary](../api/profile-post-anniversaries.md)           | [personAnniversary](personanniversary.md)                      | Создайте новый **personAnniversary,** разместив в коллекции юбилеев.               |
| [Юбилеи списка](../api/profile-list-anniversaries.md)                 | [коллекция personAnniversary](personanniversary.md)           | Получите **коллекцию объектов personAnniversary.**                                               |
| [Создание personAward](../api/profile-post-awards.md)                        | [personAward](personaward.md)                                  | Создайте новый **объект personAward,** разместив в коллекции наград.                     |
| [Награды списка](../api/profile-list-awards.md)                               | [коллекция personAward](personaward.md)                       | Получите **коллекцию объектов personAward.**                                                     |
| [Создание personCertification](../api/profile-post-certifications.md)        | [personCertification](personcertification.md)                  | Создайте новый **объект personCertification,** разместив в коллекции сертификатов.     |
| [Сертификации списков](../api/profile-list-certifications.md)               | [коллекция personCertification](personcertification.md)       | Получите **коллекцию объектов personCertification.**                                             |
| [Создание educationalActivity](../api/profile-post-educationalactivities.md) | [educationalActivity](educationalactivity.md)                  | Создайте **новую систему educationalActivity,** разместив ее в **коллекции educationalActivities.** |
| [List educationalActivities](../api/profile-list-educationalactivities.md) | [коллекция educationalActivity](educationalactivity.md)       | Получите **коллекцию объектов educationalActivity.**                                            |
| [Создание itemEmail](../api/profile-post-emails.md)                          | [itemEmail](itememail.md)                                      | Создайте новый **itemEmail,** разместив в коллекции электронных писем.                              |
| [Список сообщений электронной почты](../api/profile-list-emails.md)                               | [коллекция itemEmail](itememail.md)                           | Получите **коллекцию объектов itemEmail.**                                                      |
| [Создание personInterest](../api/profile-post-interests.md)                  | [personInterest](personinterest.md)                            | Создайте нового **человекаInterest,** разместив в коллекции интересов.                      |
| [Интересы списка](../api/profile-list-interests.md)                         | [коллекция personInterest](personinterest.md)                 | Получите **коллекцию объектов personInterest.**                                                  |
| [Создание languageProficiency](../api/profile-post-languages.md)             | [languageProficiency](languageproficiency.md)                  | Создайте **новый languageProficiency,** разместив в коллекции языков.                 |
| [Перечисление языков](../api/profile-list-languages.md)                         | [коллекция languageProficiency](languageproficiency.md)       | Получите **коллекцию объектов languageProficiency.**                                             |
| [Создание personName](../api/profile-post-names.md)                          | [personName](personname.md)                                    | Создайте новый **объект personName,** разместив в коллекции имен.                       |
| [Список имен](../api/profile-list-names.md)                                 | [коллекция personName](personname.md)                         | Получите **коллекцию объектов personName.**                                                      |
| [Создание personAnnotation](../api/profile-post-notes.md)                    | [personAnnotation](personannotation.md)                        | Создайте новый **объект personAnnotation,** разместив в коллекции заметки.                 |
| [Заметки списка](../api/profile-list-notes.md)                                 | [коллекция personAnnotation](personannotation.md)             | Получите **коллекцию объектов personAnnotation.**                                                |
| [Создание itemPatent](../api/profile-post-patents.md)                        | [itemPatent](itempatent.md)                                    | Создайте новый **объект itemPatent,** разместив в коллекции патентов.                     |
| [Патенты списка](../api/profile-list-patents.md)                             | [коллекция itemPatent](itempatent.md)                         | Получите **коллекцию объектов itemPatent.**                                                      |
| [Создание itemPhone](../api/profile-post-phones.md)                          | [itemPhone](itemphone.md)                                      | Создайте новый itemPhone, разместив в коллекции телефонов.                                  |
| [Телефоны списка](../api/profile-list-phones.md)                               | [коллекция itemPhone](itemphone.md)                           | Получите **коллекцию объектов itemPhone.**                                                       |
| [Создание workPosition](../api/profile-post-positions.md)                    | [workPosition](workposition.md)                                | Создайте новую workPosition, разместив в коллекции позиций.                            |
| [Позиции списка](../api/profile-list-positions.md)                         | [коллекция workPosition](workposition.md)                     | Получите **коллекцию объектов workPosition.**                                                    |
| [Создание projectParticipation](../api/profile-post-projects.md)             | [projectParticipation](projectparticipation.md)                | Создайте **новый projectParticipation,** разместив в коллекции проектов.                 |
| [Списки проектов](../api/profile-list-projects.md)                           | [коллекция projectParticipation](projectparticipation.md)     | Получите **коллекцию объектов projectParticipation.**                                            |
| [Создание itemPublication](../api/profile-post-publications.md)              | [itemPublication](itempublication.md)                          | Создайте новый **объект itemPublication,** разместив в коллекции публикаций.           |
| [Публикации списка](../api/profile-list-publications.md)                   | [коллекция itemPublication](itempublication.md)               | Получите **коллекцию объектов itemPublication.**                                                 |
| [Создание personResponsibility](../api/profile-post-responsibilities.md)     | [personResponsibility](personresponsibility.md)                | Создайте новый **объект personResponsibility,** разместив в коллекции обязанностей.  |
| [Обязанности списка](../api/profile-list-responsibilities.md)           | [коллекция personResponsibility](personresponsibility.md)     | Получите **коллекцию объектов personResponsibility.**                                            |
| [Создание skillProficiency](../api/profile-post-skills.md)                   | [skillProficiency](skillproficiency.md)                        | Создайте **новую skillProficiency,** разместив в коллекции навыков.                       |
| [Навыки списка](../api/profile-list-skills.md)                               | [коллекция skillProficiency](skillproficiency.md)             | Получите **коллекцию объектов skillProficiency.**                                                |
| [Создание webAccount](../api/profile-post-webaccounts.md)                    | [webAccount](webaccount.md)                                    | Создайте новый **webAccount,** разместив в коллекции webAccounts.                        |
| [Список webAccounts](../api/profile-list-webaccounts.md)                     | [коллекция webAccount](webaccount.md)                         | Получите **коллекцию объектов webAccount.**                                                      |
| [Создание personWebsite](../api/profile-post-websites.md)                    | [personWebsite](personwebsite.md)                              | Создайте новый **personWebsite,** разместив их в коллекции веб-сайтов.                        |
| [Список веб-сайтов](../api/profile-list-websites.md)                           | [коллекция personWebsite](personwebsite.md)                   | Получите **коллекцию объектов personWebsite.**                                                   |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id            |String       | Только для чтения.  |

## <a name="relationships"></a>Связи

| Связь          | Тип                                                         | Описание                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|учетные записи               |[коллекция userAccountInformation](useraccountinformation.md)| Представляет сведения, привязанные к учетной записи пользователя.                                                             |
|addresses              |[коллекция itemAddress](itemaddress.md)                      | Представляет сведения о адресах, связанных с пользователем.                                                             |
|anniversaries          |[коллекция personAnniversary](personanniversary.md)          | Представляет сведения о значимых датах, связанных с человеком.                                                                  |
|awards                 |[коллекция personAward](personaward.md)                      | Представляет сведения о наградах или почестях, связанных с человеком.                                                                  |
|certifications         |[коллекция personCertification](personcertification.md)      | Представляет сведения о сертификациях, связанных с человеком.                                                                  |
|educationalActivities  |[коллекция educationalActivity](educationalactivity.md)      | Представляет данные, предоставленные пользователем, связанными со студентами, выпускниками, аспирантами или другими образовательными мероприятиями. |
|электронные письма                 |[коллекция itemEmail](itememail.md)                          | Представляет подробные сведения о адресах электронной почты, связанных с пользователем.                       |
|interests;              |[коллекция personInterest](personinterest.md)                | Предоставляет подробные сведения об интересах пользователя, связанных с собой в различных службах.             |
|languages              |[коллекция languageProficiency](languageproficiency.md)      | Представляет подробные сведения о языках, которые пользователь добавил в свой профиль.                                    |
|names                  |[коллекция personName](personname.md)                        | Представляет имена, добавленные пользователем в свой профиль.                                    |
|notes                  |[коллекция personAnnotation](personannotation.md)            | Представляет заметки, добавленные пользователем в свой профиль.                                    |
|patents                |[коллекция itemPatent](itempatent.md)                        | Представляет патенты, добавленные пользователем в свой профиль.                                    |
|phones                 |[коллекция itemPhone](itemphone.md)                          | Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах.                            |
|позиции              |[коллекция workPosition](workposition.md)                    | Представляет подробные сведения о позициях, связанных с профилем пользователя.                                    |
|projects               |[коллекция projectParticipation](projectparticipation.md)    | Представляет подробные сведения о проектах, связанных с пользователем.                                                     |
|publications           |[коллекция itemPublication](itempublication.md)              | Представляет сведения о любых публикациях, добавленных пользователем в свой профиль.                                                     |
|responsibilities;       |[коллекция personResponsibility](personResponsibility.md)    | Представляет сведения об обязанностях, которые пользователь добавил в свой профиль.                                                     |
|skills.                 |[коллекция skillProficiency](skillproficiency.md)            | Представляет подробные сведения о навыках, связанных с пользователем в различных службах.                                   |
|webAccounts            |[коллекция webAccount](webaccount.md)                        | Представляет веб-учетные записи, которые пользователь указал, что использует или добавил в свой профиль пользователя.                               |
|websites               |[коллекция personWebsite](personwebsite.md)                  | Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах.                                 |

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


