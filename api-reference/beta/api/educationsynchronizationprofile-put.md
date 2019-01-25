---
title: Обновление educationSynchronizationProfile
description: Обновляет свойства существующего профиля синхронизации данных school в клиентов.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 668aad65abe2c9b3d4609400118f9341748210f1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510577"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="cb3c7-103">Обновление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="cb3c7-103">Update an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb3c7-104">Обновление свойств существующих данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-104">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb3c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb3c7-105">Permissions</span></span>
<span data-ttu-id="cb3c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cb3c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cb3c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cb3c7-108">Permission type</span></span> | <span data-ttu-id="cb3c7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cb3c7-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="cb3c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cb3c7-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cb3c7-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="cb3c7-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="cb3c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cb3c7-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="cb3c7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-113">Not supported.</span></span>|
|<span data-ttu-id="cb3c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cb3c7-114">Application</span></span>|<span data-ttu-id="cb3c7-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb3c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cb3c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="cb3c7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cb3c7-117">Request headers</span></span>
| <span data-ttu-id="cb3c7-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cb3c7-118">Name</span></span>       | <span data-ttu-id="cb3c7-119">Тип</span><span class="sxs-lookup"><span data-stu-id="cb3c7-119">Type</span></span> | <span data-ttu-id="cb3c7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="cb3c7-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cb3c7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb3c7-121">Authorization</span></span>  | <span data-ttu-id="cb3c7-122">string</span><span class="sxs-lookup"><span data-stu-id="cb3c7-122">string</span></span>  | <span data-ttu-id="cb3c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cb3c7-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb3c7-125">Content-Type</span></span> | <span data-ttu-id="cb3c7-126">string</span><span class="sxs-lookup"><span data-stu-id="cb3c7-126">string</span></span> | <span data-ttu-id="cb3c7-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cb3c7-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cb3c7-129">Request body</span></span>
<span data-ttu-id="cb3c7-130">В тексте запроса укажите представление объекта [synchronizationProfile](../resources/educationsynchronizationprofile.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-130">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cb3c7-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb3c7-131">Response</span></span>
<span data-ttu-id="cb3c7-132">Успешно завершена, этот метод возвращает `202, Accepted` код ответа и объект [synchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-132">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cb3c7-133">Пример</span><span class="sxs-lookup"><span data-stu-id="cb3c7-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cb3c7-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="cb3c7-134">Request</span></span>
<span data-ttu-id="cb3c7-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_synchronizationProfile"
}-->
```http
PUT https://graph.microsoft.com/beta/education/synchronizationProfiles
Content-type: application/json

{
    "displayName": "Test Profile",
    "dataProvider": {
        "@odata.type": "microsoft.graph.educationcsvdataprovider",
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
        "@odata.type": "microsoft.graph.educationidentitycreationconfiguration",
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

##### <a name="response"></a><span data-ttu-id="cb3c7-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="cb3c7-136">Response</span></span>
<span data-ttu-id="cb3c7-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-137">Here is an example of the response.</span></span> 

><span data-ttu-id="cb3c7-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cb3c7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
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
    "Error: /api-reference/beta/api/educationsynchronizationprofile-put.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
