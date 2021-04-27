---
title: Обновление educationSynchronizationProfile
description: Обновление свойств существующего профиля синхронизации школьных данных в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 675cf90ed375bd157f10d0268eef3b90bf3edf5b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52042952"
---
# <a name="update-an-educationsynchronizationprofile"></a><span data-ttu-id="27dcc-103">Обновление educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="27dcc-103">Update an educationSynchronizationProfile</span></span>

<span data-ttu-id="27dcc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27dcc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="27dcc-105">Обновление свойств существующего профиля синхронизации [школьных](../resources/educationsynchronizationprofile.md) данных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="27dcc-105">Update properties for an existing school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="27dcc-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27dcc-106">Permissions</span></span>
<span data-ttu-id="27dcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27dcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27dcc-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27dcc-109">Permission type</span></span> | <span data-ttu-id="27dcc-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27dcc-110">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="27dcc-111">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27dcc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="27dcc-112">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27dcc-112">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="27dcc-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="27dcc-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="27dcc-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27dcc-114">Not supported.</span></span>|
|<span data-ttu-id="27dcc-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="27dcc-115">Application</span></span>|<span data-ttu-id="27dcc-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27dcc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27dcc-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27dcc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /education/synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="27dcc-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27dcc-118">Request headers</span></span>
| <span data-ttu-id="27dcc-119">Имя</span><span class="sxs-lookup"><span data-stu-id="27dcc-119">Name</span></span>       | <span data-ttu-id="27dcc-120">Тип</span><span class="sxs-lookup"><span data-stu-id="27dcc-120">Type</span></span> | <span data-ttu-id="27dcc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="27dcc-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="27dcc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27dcc-122">Authorization</span></span>  | <span data-ttu-id="27dcc-123">string</span><span class="sxs-lookup"><span data-stu-id="27dcc-123">string</span></span>  | <span data-ttu-id="27dcc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27dcc-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="27dcc-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="27dcc-126">Content-Type</span></span> | <span data-ttu-id="27dcc-127">string</span><span class="sxs-lookup"><span data-stu-id="27dcc-127">string</span></span> | <span data-ttu-id="27dcc-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27dcc-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="27dcc-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27dcc-130">Request body</span></span>
<span data-ttu-id="27dcc-131">В теле запроса поставляем представление JSON объекта [synchronizationProfile.](../resources/educationsynchronizationprofile.md)</span><span class="sxs-lookup"><span data-stu-id="27dcc-131">In the request body, supply a JSON representation of the [synchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="27dcc-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="27dcc-132">Response</span></span>
<span data-ttu-id="27dcc-133">В случае успешной работы этот метод возвращает код отклика и объект `202, Accepted` [синхронизацииProfile](../resources/educationsynchronizationprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="27dcc-133">If successful, this method returns a `202, Accepted` response code and a [synchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27dcc-134">Пример</span><span class="sxs-lookup"><span data-stu-id="27dcc-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27dcc-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="27dcc-135">Request</span></span>
<span data-ttu-id="27dcc-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27dcc-136">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="27dcc-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="27dcc-137">Response</span></span>
<span data-ttu-id="27dcc-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27dcc-138">Here is an example of the response.</span></span> 

><span data-ttu-id="27dcc-139">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="27dcc-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


