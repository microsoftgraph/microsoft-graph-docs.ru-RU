---
title: Тип ресурса Profile
description: Представляет свойства, которые являются описательными для пользователя и доступны для совместного использования, люди в Microsoft 365 и сторонние службы и возможности с помощью Microsoft Graph.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1f80dfccbd662e1e398c0d4b79b0086575a83e2b
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050893"
---
# <a name="profile-resource-type"></a>Тип ресурса Profile

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет свойства, которые являются описательными для пользователя в клиенте, например юбилеев и действия по образованию. Эти свойства задаются совместно с другими пользователями в Microsoft 365, а сторонние службы и возможности — с помощью Microsoft Graph. 

Программным способом эти свойства выражаются в виде [связей](#relationships) ресурса **профиля** . Чтобы получить одно из этих свойств навигации или создать экземпляр этих свойств для пользователя, используйте соответствующий метод GET или POST для этого свойства там, где это уместно. Ознакомьтесь с приведенными ниже [способами](#methods) .

## <a name="methods"></a>Методы

| Метод                                                                     | Возвращаемый тип                                                    | Описание                                                                                  |
|:---------------------------------------------------------------------------|:---------------------------------------------------------------|:---------------------------------------------------------------------------------------------|
| [Получение профиля](../api/profile-get.md)                                       | [profile](profile.md)                                          | Чтение свойств и связей объекта Profile.                                         |
| [Удаление профиля](../api/profile-delete.md)                                 | Нет                                                           | Удаление объекта **Profile** .                                                                 |
| [Учетная запись списка](../api/profile-list-account.md)                             | Коллекция [усераккаунтинформатион](useraccountinformation.md) | Получение коллекции объектов **усераккаунтинформатион** .                                          |
| [Создание Персонанниверсари](../api/profile-post-anniversaries.md)           | [персонанниверсари](personanniversary.md)                      | Создание нового **персонанниверсари** путем публикации в коллекции юбилеев.               |
| [Список юбилеев](../api/profile-list-anniversaries.md)                 | Коллекция [персонанниверсари](personanniversary.md)           | Получение коллекции объектов **персонанниверсари** .                                               |
| [Создание Едукатионалактивити](../api/profile-post-educationalactivities.md) | [едукатионалактивити](educationalactivity.md)                  | Создание нового **едукатионалактивити** путем отправки в коллекцию **едукатионалактивитиес** . |
| [Список Едукатионалактивитиес](../api/profile-list-educationalactivities.md) | Коллекция [едукатионалактивити](educationalactivity.md)       | Получение коллекции объектов **едукатионалактивити** .                                            |
| [Создание Итемемаил](../api/profile-post-emails.md)                          | [итемемаил](itememail.md)                                      | Создание нового **итемемаил** путем отправки в коллекцию сообщений электронной почты.                              |
| [Список сообщений электронной почты](../api/profile-list-emails.md)                               | Коллекция [итемемаил](itememail.md)                           | Получение коллекции объектов **итемемаил** .                                                      |
| [Создание Персонинтерест](../api/profile-post-interests.md)                  | [персонинтерест](personinterest.md)                            | Создание нового **персонинтерест** путем отправки в коллекцию интересов.                      |
| [Список интересов](../api/profile-list-interests.md)                         | Коллекция [персонинтерест](personinterest.md)                 | Получение коллекции объектов **персонинтерест** .                                                  |
| [Создание ЛангуажепрофиЦиенци](../api/profile-post-languages.md)             | [лангуажепрофиЦиенци](languageproficiency.md)                  | Создание нового **лангуажепрофиЦиенци** путем публикации в коллекции Languages.                 |
| [Список языков](../api/profile-list-languages.md)                         | Коллекция [лангуажепрофиЦиенци](languageproficiency.md)       | Получение коллекции объектов **лангуажепрофиЦиенци** .                                             |
| [Список имен](../api/profile-list-names.md)                                 | Коллекция [PersonName](personname.md)                         | Получение коллекции объектов **PersonName** .                                                      |
| [Создание personName](../api/profile-post-names.md)                          | [personName](personName.md)                                    | Создайте новый объект **PersonName** , отправив его в коллекцию Names.                       |
| [Список веб-сайтов](../api/profile-list-websites.md)                           | Коллекция [персонвебсите](personwebsite.md)                   | Получение коллекции объектов **персонвебсите** .                                                   |
| [Создание Итемфоне](../api/profile-post-phones.md)                          | [итемфоне](itemphone.md)                                      | Создание нового Итемфоне путем публикации в коллекции phones.                                  |
| [Перечисление телефонов](../api/profile-list-phones.md)                               | Коллекция [итемфоне](itemphone.md)                           | Получение коллекции объектов **итемфоне** .                                                       |
| [Создание Воркпоситион](../api/profile-post-positions.md)                    | [воркпоситион](workposition.md)                                | Создание нового Воркпоситион путем отправки в коллекцию Positions.                            |
| [Позиции списка](../api/profile-list-positions.md)                         | Коллекция [воркпоситион](workposition.md)                     | Получение коллекции объектов **воркпоситион** .                                                    |
| [Создание ПрожектпартиЦипатион](../api/profile-post-projects.md)             | [прожектпартиЦипатион](projectparticipation.md)                | Создание нового **прожектпартиЦипатион** путем публикации в коллекции проектов.                 |
| [Список проектов](../api/profile-list-projects.md)                           | Коллекция [прожектпартиЦипатион](projectparticipation.md)     | Получение коллекции объектов **прожектпартиЦипатион** .                                            |
| [Создание СкиллпрофиЦиенци](../api/profile-post-skills.md)                   | [скиллпрофиЦиенци](skillproficiency.md)                        | Создание нового **скиллпрофиЦиенци** путем публикации в коллекции навыков.                       |
| [Список навыков](../api/profile-list-skills.md)                               | Коллекция [скиллпрофиЦиенци](skillproficiency.md)             | Получение коллекции объектов **скиллпрофиЦиенци** .                                                |
| [Создание учетной записи](../api/profile-post-webaccounts.md)                    | [Учетная запись учетной записи](webaccount.md)                                    | Создайте новую **учетную запись** , разместив ее в коллекции учетных записей.                        |
| [Список учетных записей](../api/profile-list-webaccounts.md)                     | Коллекция [учетных записей](webaccount.md)                         | Получение коллекции объектов **учетных записей** .                                                      |
| [Создание Персонвебсите](../api/profile-post-websites.md)                    | [персонвебсите](personwebsite.md)                              | Создание нового **персонвебсите** путем публикации в семействе веб-сайтов.                        |
| [Список веб-сайтов](../api/profile-list-websites.md)                           | Коллекция [персонвебсите](personwebsite.md)                   | Получение коллекции объектов **персонвебсите** .                                                   |

## <a name="properties"></a>Свойства

| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id            |String       | Только для чтения.  |

## <a name="relationships"></a>Отношения

| Связь          | Тип                                                         | Описание                                                                                                                                    |
|:----------------------|:-------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
|финансового                |Коллекция [усераккаунтинформатион](useraccountinformation.md)| Представляет сведения, специально связанные с учетной записью пользователя. Только для чтения. Допускается значение null.                                                             |
|годовщины          |Коллекция [персонанниверсари](personanniversary.md)          | Представляет сведения о значимых датах, связанных с пользователем. Только для чтения. Допускается значение null.                                                      |
|едукатионалактивитиес  |Коллекция [едукатионалактивити](educationalactivity.md)      | Представляет данные, которые пользователь предоставил, относящихся к выпуску, выпускнику, выпуску или другим учебным действиям. Только для чтения. Допускается значение null.|
|письма                 |Коллекция [итемемаил](itememail.md)                          | Представляет подробные сведения об адресах электронной почты, связанных с пользователем. Только для чтения. Допускается значение null.                                           |
|interests;              |Коллекция [персонинтерест](personinterest.md)                | Предоставляет подробные сведения о интересах, которые пользователь связал с собственными службами в различных службах. Только для чтения. Допускается значение null.                |
|Языки              |Коллекция [лангуажепрофиЦиенци](languageproficiency.md)      | Представляет подробные сведения о языках, добавленных пользователем в свой профиль. Только для чтения. Допускается значение null.                                   |
|phones                 |Коллекция [итемфоне](itemphone.md)                          | Представляет подробные сведения о номерах телефонов, связанных с пользователем в различных службах. Только для чтения. Допускается значение null.                           |
|расположен              |Коллекция [воркпоситион](workposition.md)                    | Представляет подробные сведения о должностных единицах, связанных с профилем пользователя. Только для чтения. Допускается значение null.                                    |
|projects               |Коллекция [прожектпартиЦипатион](projectparticipation.md)    | Представляет подробные сведения о проектах, связанных с пользователем. Только для чтения. Допускается значение null.                                                    |
|skills.                 |Коллекция [скиллпрофиЦиенци](skillproficiency.md)            | Представляет подробные сведения о навыках, связанных с пользователем в различных службах. Только для чтения. Допускается значение null.                                  |
|Учетные записи учетных записей            |Коллекция [учетных записей](webaccount.md)                        | Представляет веб-учетные записи, которые пользователь указал, используют или добавили в свой профиль пользователя. Только для чтения. Допускается значение null.                               |
|websites               |Коллекция [персонвебсите](personwebsite.md)                  | Представляет подробные сведения о веб-сайтах, связанных с пользователем в различных службах. Только для чтения. Допускается значение null.                                |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profile",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
    "id": "String (identifier)"
}
```

<!--
{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
-->


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
