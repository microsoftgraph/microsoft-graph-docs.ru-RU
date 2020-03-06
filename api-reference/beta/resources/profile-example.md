---
title: Использование API профилей в Microsoft Graph для получения информации об определенном пользователе или о себе
description: 'Приложения Microsoft Graph могут получать данные профиля других пользователей с помощью API профилей. '
author: kevinbellinger
localization_priority: Priority
ms.prod: people
doc_type: conceptualPageType
ms.openlocfilehash: e0a402cd01cf9dc8effd16496d7230cc8e98d5d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521476"
---
# <a name="use-the-profile-api-in-microsoft-graph-to-retrieve-information-about-yourself-or-another-user"></a><span data-ttu-id="41581-103">Использование API профилей в Microsoft Graph для получения информации о себе или другом пользователе</span><span class="sxs-lookup"><span data-stu-id="41581-103">Use the Profile API in Microsoft Graph to retrieve information about yourself or another user</span></span> 

<span data-ttu-id="41581-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41581-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41581-105">Приложения Microsoft Graph могут использовать API профилей для получения профиля вошедшего или другого пользователя с помощью действительной учетной записи Майкрософт или Azure AD.</span><span class="sxs-lookup"><span data-stu-id="41581-105">Microsoft Graph applications can use the Profile API to retrieve the profile of the signed-in user or another user with a valid Azure AD or Microsoft account.</span></span> <span data-ttu-id="41581-106">Эту информацию можно использовать в приложениях, чтобы помочь получить контекстные сведения о другом пользователе, расширить возможности пользователя приложения или реализовать механизм хранения расширенной информации о пользователе, который также можно использовать в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="41581-106">This information can be used in applications to assist in contextualizing another user, providing a richer experience for the user within the application or as a mechanism for storing extended information about the user which can also be used within Microsoft 365.</span></span> 

## <a name="authorization"></a><span data-ttu-id="41581-107">Авторизация</span><span class="sxs-lookup"><span data-stu-id="41581-107">Authorization</span></span>

<span data-ttu-id="41581-108">Чтобы ваше приложение в Microsoft Graph могло вызывать API People, ему потребуются указанные ниже разрешения.</span><span class="sxs-lookup"><span data-stu-id="41581-108">To call the People API in Microsoft Graph, your app will need the appropriate permissions:</span></span>

* <span data-ttu-id="41581-109">User.Read — используется для отправки общих вызовов API профилей. Пример: `https://graph.microsoft.com/beta/me/profile/`.</span><span class="sxs-lookup"><span data-stu-id="41581-109">User.Read - Use to make general Profile API calls; for example, `https://graph.microsoft.com/beta/me/profile/`.</span></span> <span data-ttu-id="41581-110">Для использования разрешения User.Read требуется согласие пользователя.</span><span class="sxs-lookup"><span data-stu-id="41581-110">User.Read requires end user consent.</span></span>

## <a name="view-my-profile"></a><span data-ttu-id="41581-111">Просмотр моего профиля</span><span class="sxs-lookup"><span data-stu-id="41581-111">View my profile</span></span>

<span data-ttu-id="41581-112">С помощью описанных в этом разделе запросов можно получить данные о людях, наиболее релевантных для пользователя, выполнившего вход в систему (`/me`).</span><span class="sxs-lookup"><span data-stu-id="41581-112">The requests in this section get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="41581-113">Для выполнения этих запросов у вошедшего пользователя должно быть разрешение User.Read.</span><span class="sxs-lookup"><span data-stu-id="41581-113">These requests require the User.Read permission to be present for the signed-in user.</span></span> 


```http
GET https://graph.microsoft.com/beta/me/profile/
```

<span data-ttu-id="41581-p104">В примере ниже показан отклик. По умолчанию в каждом отклике возвращается 10 записей. Вы можете изменить количество возвращаемых записей с помощью параметра запроса *$top*. В этом примере показано, как использовать параметр запроса *$top* для ограничения количества записей (до 3 шт.) в отклике.</span><span class="sxs-lookup"><span data-stu-id="41581-p104">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```
