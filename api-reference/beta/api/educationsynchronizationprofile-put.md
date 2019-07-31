---
title: Обновление Едукатионсинчронизатионпрофиле
description: Обновление свойств существующего профиля синхронизации данных School в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 9535da9fa454b9a416779e5157200a178b647d37
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954818"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="077e5-103">Обновление Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="077e5-103">Update an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="077e5-104">Обновление свойств существующего [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="077e5-104">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="077e5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="077e5-105">Permissions</span></span>
<span data-ttu-id="077e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="077e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="077e5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="077e5-108">Permission type</span></span> | <span data-ttu-id="077e5-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="077e5-109">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="077e5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="077e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="077e5-111">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="077e5-111">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="077e5-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="077e5-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="077e5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="077e5-113">Not supported.</span></span>|
|<span data-ttu-id="077e5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="077e5-114">Application</span></span>|<span data-ttu-id="077e5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="077e5-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="077e5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="077e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="077e5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="077e5-117">Request headers</span></span>
| <span data-ttu-id="077e5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="077e5-118">Name</span></span>       | <span data-ttu-id="077e5-119">Тип</span><span class="sxs-lookup"><span data-stu-id="077e5-119">Type</span></span> | <span data-ttu-id="077e5-120">Описание</span><span class="sxs-lookup"><span data-stu-id="077e5-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="077e5-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="077e5-121">Authorization</span></span>  | <span data-ttu-id="077e5-122">string</span><span class="sxs-lookup"><span data-stu-id="077e5-122">string</span></span>  | <span data-ttu-id="077e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="077e5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="077e5-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="077e5-125">Content-Type</span></span> | <span data-ttu-id="077e5-126">string</span><span class="sxs-lookup"><span data-stu-id="077e5-126">string</span></span> | <span data-ttu-id="077e5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="077e5-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="077e5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="077e5-129">Request body</span></span>
<span data-ttu-id="077e5-130">В тексте запроса добавьте представление объекта [синчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="077e5-130">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="077e5-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="077e5-131">Response</span></span>
<span data-ttu-id="077e5-132">В случае успешного выполнения этот метод возвращает `202, Accepted` код отклика и объект [синчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="077e5-132">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="077e5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="077e5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="077e5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="077e5-134">Request</span></span>
<span data-ttu-id="077e5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="077e5-135">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="077e5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="077e5-136">Response</span></span>
<span data-ttu-id="077e5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="077e5-137">Here is an example of the response.</span></span> 

><span data-ttu-id="077e5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="077e5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
