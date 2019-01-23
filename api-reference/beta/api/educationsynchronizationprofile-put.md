---
title: Обновление educationSynchronizationProfile
description: Обновляет свойства существующего профиля синхронизации данных school в клиентов.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 0c99984b4ca0d8d72fdc02d28a8de80761fdbd60
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398739"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="ab35d-103">Обновление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="ab35d-103">Update an educationSynchronizationProfile</span></span>

> <span data-ttu-id="ab35d-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab35d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab35d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab35d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab35d-106">Обновление свойств существующих данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="ab35d-106">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab35d-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab35d-107">Permissions</span></span>
<span data-ttu-id="ab35d-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab35d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ab35d-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab35d-110">Permission type</span></span> | <span data-ttu-id="ab35d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab35d-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="ab35d-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab35d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab35d-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ab35d-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="ab35d-114">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="ab35d-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="ab35d-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab35d-115">Not supported.</span></span>|
|<span data-ttu-id="ab35d-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab35d-116">Application</span></span>|<span data-ttu-id="ab35d-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab35d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab35d-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab35d-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ab35d-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab35d-119">Request headers</span></span>
| <span data-ttu-id="ab35d-120">Имя</span><span class="sxs-lookup"><span data-stu-id="ab35d-120">Name</span></span>       | <span data-ttu-id="ab35d-121">Тип</span><span class="sxs-lookup"><span data-stu-id="ab35d-121">Type</span></span> | <span data-ttu-id="ab35d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ab35d-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ab35d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab35d-123">Authorization</span></span>  | <span data-ttu-id="ab35d-124">string</span><span class="sxs-lookup"><span data-stu-id="ab35d-124">string</span></span>  | <span data-ttu-id="ab35d-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab35d-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ab35d-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ab35d-127">Content-Type</span></span> | <span data-ttu-id="ab35d-128">строка</span><span class="sxs-lookup"><span data-stu-id="ab35d-128">string</span></span> | <span data-ttu-id="ab35d-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ab35d-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab35d-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ab35d-131">Request body</span></span>
<span data-ttu-id="ab35d-132">В тексте запроса укажите представление объекта [synchronizationProfile](../resources/educationsynchronizationprofile.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="ab35d-132">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ab35d-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab35d-133">Response</span></span>
<span data-ttu-id="ab35d-134">Успешно завершена, этот метод возвращает `202, Accepted` код ответа и объект [synchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="ab35d-134">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab35d-135">Пример</span><span class="sxs-lookup"><span data-stu-id="ab35d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab35d-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="ab35d-136">Request</span></span>
<span data-ttu-id="ab35d-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ab35d-137">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="ab35d-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="ab35d-138">Response</span></span>
<span data-ttu-id="ab35d-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ab35d-139">Here is an example of the response.</span></span> 

><span data-ttu-id="ab35d-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ab35d-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
