---
title: Обновление educationSynchronizationProfile
description: Обновляет свойства существующего профиля синхронизации данных school в клиентов.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 07947127b0346a33528136921580646623576d28
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935089"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="9555e-103">Обновление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="9555e-103">Update an educationSynchronizationProfile</span></span>

> <span data-ttu-id="9555e-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9555e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9555e-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9555e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9555e-106">Обновление свойств существующих данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="9555e-106">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="9555e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9555e-107">Permissions</span></span>
<span data-ttu-id="9555e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9555e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9555e-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9555e-110">Permission type</span></span> | <span data-ttu-id="9555e-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="9555e-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="9555e-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9555e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9555e-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9555e-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="9555e-114">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="9555e-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="9555e-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9555e-115">Not supported.</span></span>|
|<span data-ttu-id="9555e-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9555e-116">Application</span></span>|<span data-ttu-id="9555e-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9555e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9555e-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9555e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="9555e-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9555e-119">Request headers</span></span>
| <span data-ttu-id="9555e-120">Имя</span><span class="sxs-lookup"><span data-stu-id="9555e-120">Name</span></span>       | <span data-ttu-id="9555e-121">Тип</span><span class="sxs-lookup"><span data-stu-id="9555e-121">Type</span></span> | <span data-ttu-id="9555e-122">Описание</span><span class="sxs-lookup"><span data-stu-id="9555e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9555e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9555e-123">Authorization</span></span>  | <span data-ttu-id="9555e-124">string</span><span class="sxs-lookup"><span data-stu-id="9555e-124">string</span></span>  | <span data-ttu-id="9555e-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9555e-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9555e-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9555e-127">Content-Type</span></span> | <span data-ttu-id="9555e-128">строка</span><span class="sxs-lookup"><span data-stu-id="9555e-128">string</span></span> | <span data-ttu-id="9555e-p104">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9555e-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9555e-131">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9555e-131">Request body</span></span>
<span data-ttu-id="9555e-132">В тексте запроса укажите представление объекта [synchronizationProfile](../resources/educationsynchronizationprofile.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="9555e-132">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="9555e-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9555e-133">Response</span></span>
<span data-ttu-id="9555e-134">Успешно завершена, этот метод возвращает `202, Accepted` код ответа и объект [synchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9555e-134">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9555e-135">Пример</span><span class="sxs-lookup"><span data-stu-id="9555e-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9555e-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="9555e-136">Request</span></span>
<span data-ttu-id="9555e-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9555e-137">Here is an example of the request.</span></span>
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
        "@odata.type": "#microsoft.graph.educationcsvdataprovider",
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
        "@odata.type": "#microsoft.graph.educationidentitycreationconfiguration",
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

##### <a name="response"></a><span data-ttu-id="9555e-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="9555e-138">Response</span></span>
<span data-ttu-id="9555e-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9555e-139">Here is an example of the response.</span></span> 

><span data-ttu-id="9555e-p105">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="9555e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "displayName": "Test Profile",
    "state": "provisioning",
    "id": "86904b1e-c7d0-4ead-b13a-98f11fc400ee",
    "dataProvider": {
        "@odata.type": "#microsoft.graph.educationCsvDataProvider",
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
        "@odata.type": "#microsoft.graph.educationIdentityCreationConfiguration",
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
            "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",                
            "appliesTo": "teacher",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        },
        {
            "@odata.type": "#microsoft.graph.educationSynchronizationLicenseAssignment",                
            "appliesTo": "student",
            "skuIds": [
                "6fd2c87f-b296-42f0-b197-1e91e994b900"
            ]
        }
    ]
}
```
