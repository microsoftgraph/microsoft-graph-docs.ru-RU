---
title: Создание educationSynchronizationProfile
description: 'Создание запроса для школа данных синхронизации профиля в клиентов. Запрос состояния, чтобы получить сведения о состоянии профиля. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: efc9b76405b57d0e47d645d0e7b00dc9425ba71b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520818"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="ea14f-104">Создание educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="ea14f-104">Create an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea14f-105">Создание запроса для нового данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="ea14f-105">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="ea14f-106">[Запрос состояния](educationsynchronizationprofilestatus-get.md) , чтобы получить сведения о состоянии профиля.</span><span class="sxs-lookup"><span data-stu-id="ea14f-106">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="ea14f-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea14f-107">Permissions</span></span>
<span data-ttu-id="ea14f-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ea14f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea14f-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ea14f-110">Permission type</span></span> | <span data-ttu-id="ea14f-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ea14f-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ea14f-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ea14f-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ea14f-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ea14f-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ea14f-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ea14f-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ea14f-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea14f-115">Not supported.</span></span>|
|<span data-ttu-id="ea14f-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ea14f-116">Application</span></span>|<span data-ttu-id="ea14f-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea14f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea14f-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ea14f-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ea14f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ea14f-119">Request headers</span></span>
| <span data-ttu-id="ea14f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ea14f-120">Name</span></span>       | <span data-ttu-id="ea14f-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ea14f-121">Type</span></span> | <span data-ttu-id="ea14f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ea14f-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ea14f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea14f-123">Authorization</span></span>  | <span data-ttu-id="ea14f-124">string</span><span class="sxs-lookup"><span data-stu-id="ea14f-124">string</span></span>  | <span data-ttu-id="ea14f-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea14f-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ea14f-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ea14f-127">Content-Type</span></span> | <span data-ttu-id="ea14f-128">string</span><span class="sxs-lookup"><span data-stu-id="ea14f-128">string</span></span> | <span data-ttu-id="ea14f-129">application/json</span><span class="sxs-lookup"><span data-stu-id="ea14f-129">Application/json.</span></span> <span data-ttu-id="ea14f-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ea14f-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea14f-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ea14f-131">Request body</span></span>
<span data-ttu-id="ea14f-132">В тексте запроса укажите представление объекта [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="ea14f-132">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ea14f-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea14f-133">Response</span></span>
<span data-ttu-id="ea14f-134">Успешно завершена, этот метод возвращает `202, Accepted` код ответа и объект [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ea14f-134">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea14f-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ea14f-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea14f-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ea14f-136">Request</span></span>
<span data-ttu-id="ea14f-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ea14f-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationSynchronizationProfile"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ]
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationIdentitySynchronizationConfiguration",
        "userDomains": [
            {
                "appliesTo": "student",
                "name": "testschool.edu"
            },
            {
                "appliesTo": "teacher",
                "name": "testschool.edu"
            }
        ]
    },
    "licensesToAssign": [
        {
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```

##### <a name="response"></a><span data-ttu-id="ea14f-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="ea14f-138">Response</span></span>
<span data-ttu-id="ea14f-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ea14f-139">The following is an example of the response.</span></span> 

><span data-ttu-id="ea14f-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ea14f-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationCsvDataProvider",
        "customizations": {
            "student": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Middle Name"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacher": {
                "optionalPropertiesToSync": [
                    "State ID",
                    "Teacher Number",
                    "Status",
                    "Middle Name",
                    "Secondary Email",
                    "Title",
                    "Qualification"
                ],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "studentEnrollment": {
                "optionalPropertiesToSync": [],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            },
            "teacherRoster": {
                "optionalPropertiesToSync": [],
                "synchronizationStartDate": "0001-01-01T00:00:00Z",
                "isSyncDeferred": false,
                "allowDisplayNameUpdate": false
            }
        }
    },
    "identitySynchronizationConfiguration": {
        "@odata.type": "microsoft.graph.educationIdentityCreationConfiguration",
        "userDomains": [
            {
                "appliesTo": "student",
                "name": "testschool.edu"
            },
            {
                "appliesTo": "teacher",
                "name": "testschool.edu"
            }
        ]
    },
    "licensesToAssign": [
        {
            "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "@odata.type": "microsoft.graph.educationSynchronizationLicenseAssignment",
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
