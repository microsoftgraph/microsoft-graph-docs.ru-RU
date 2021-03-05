---
title: Создание educationSynchronizationProfile
description: 'Создайте запрос для нового профиля синхронизации школьных данных в клиенте. Запрос состояния, чтобы получить состояние профиля. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f84d4f66036d3f767182c5e7abf12c231699073f
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470237"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="fcda9-104">Создание educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="fcda9-104">Create an educationSynchronizationProfile</span></span>

<span data-ttu-id="fcda9-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcda9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fcda9-106">Создайте запрос для нового профиля синхронизации [школьных](../resources/educationsynchronizationprofile.md) данных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="fcda9-106">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="fcda9-107">[Запрос состояния,](educationsynchronizationprofilestatus-get.md) чтобы получить состояние профиля.</span><span class="sxs-lookup"><span data-stu-id="fcda9-107">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fcda9-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcda9-108">Permissions</span></span>
<span data-ttu-id="fcda9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fcda9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fcda9-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fcda9-111">Permission type</span></span> | <span data-ttu-id="fcda9-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fcda9-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="fcda9-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fcda9-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fcda9-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fcda9-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="fcda9-115">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fcda9-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fcda9-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcda9-116">Not supported.</span></span>|
|<span data-ttu-id="fcda9-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fcda9-117">Application</span></span>|<span data-ttu-id="fcda9-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fcda9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcda9-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fcda9-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="fcda9-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fcda9-120">Request headers</span></span>
| <span data-ttu-id="fcda9-121">Имя</span><span class="sxs-lookup"><span data-stu-id="fcda9-121">Name</span></span>       | <span data-ttu-id="fcda9-122">Тип</span><span class="sxs-lookup"><span data-stu-id="fcda9-122">Type</span></span> | <span data-ttu-id="fcda9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="fcda9-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fcda9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcda9-124">Authorization</span></span>  | <span data-ttu-id="fcda9-125">string</span><span class="sxs-lookup"><span data-stu-id="fcda9-125">string</span></span>  | <span data-ttu-id="fcda9-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fcda9-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fcda9-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fcda9-128">Content-Type</span></span> | <span data-ttu-id="fcda9-129">string</span><span class="sxs-lookup"><span data-stu-id="fcda9-129">string</span></span> | <span data-ttu-id="fcda9-130">Application/json.</span><span class="sxs-lookup"><span data-stu-id="fcda9-130">Application/json.</span></span> <span data-ttu-id="fcda9-131">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="fcda9-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fcda9-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fcda9-132">Request body</span></span>
<span data-ttu-id="fcda9-133">В теле запроса поставляем представление JSON объекта [educationSynchronizationProfile.](../resources/educationsynchronizationprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fcda9-133">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fcda9-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcda9-134">Response</span></span>
<span data-ttu-id="fcda9-135">В случае успеха этот метод возвращает код отклика и `202, Accepted` [объект educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fcda9-135">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcda9-136">Пример</span><span class="sxs-lookup"><span data-stu-id="fcda9-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fcda9-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="fcda9-137">Request</span></span>
<span data-ttu-id="fcda9-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fcda9-138">The following is an example of the request.</span></span>
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
        "@odata.type": "#Microsoft.Education.DataSync.educationCsvDataProvider",
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
        "@odata.type": "#Microsoft.Education.DataSync.educationIdentityCreationConfiguration",
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

##### <a name="response"></a><span data-ttu-id="fcda9-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="fcda9-139">Response</span></span>
<span data-ttu-id="fcda9-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fcda9-140">The following is an example of the response.</span></span> 

><span data-ttu-id="fcda9-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fcda9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
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


