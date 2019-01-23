---
title: Создание educationSynchronizationProfile
description: 'Создание запроса для школа данных синхронизации профиля в клиентов. Запрос состояния, чтобы получить сведения о состоянии профиля. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 4a8864979254eaafdb71b3524831227399d7bff6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417877"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="fe5ba-104">Создание educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="fe5ba-104">Create an educationSynchronizationProfile</span></span>

> <span data-ttu-id="fe5ba-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe5ba-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe5ba-107">Создание запроса для нового данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-107">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="fe5ba-108">[Запрос состояния](educationsynchronizationprofilestatus-get.md) , чтобы получить сведения о состоянии профиля.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-108">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fe5ba-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe5ba-109">Permissions</span></span>
<span data-ttu-id="fe5ba-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fe5ba-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fe5ba-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fe5ba-112">Permission type</span></span> | <span data-ttu-id="fe5ba-113">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fe5ba-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="fe5ba-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fe5ba-114">Delegated (work or school account)</span></span> | <span data-ttu-id="fe5ba-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fe5ba-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="fe5ba-116">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="fe5ba-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="fe5ba-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-117">Not supported.</span></span>|
|<span data-ttu-id="fe5ba-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fe5ba-118">Application</span></span>|<span data-ttu-id="fe5ba-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe5ba-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fe5ba-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="fe5ba-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fe5ba-121">Request headers</span></span>
| <span data-ttu-id="fe5ba-122">Имя</span><span class="sxs-lookup"><span data-stu-id="fe5ba-122">Name</span></span>       | <span data-ttu-id="fe5ba-123">Тип</span><span class="sxs-lookup"><span data-stu-id="fe5ba-123">Type</span></span> | <span data-ttu-id="fe5ba-124">Описание</span><span class="sxs-lookup"><span data-stu-id="fe5ba-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe5ba-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe5ba-125">Authorization</span></span>  | <span data-ttu-id="fe5ba-126">string</span><span class="sxs-lookup"><span data-stu-id="fe5ba-126">string</span></span>  | <span data-ttu-id="fe5ba-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fe5ba-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe5ba-129">Content-Type</span></span> | <span data-ttu-id="fe5ba-130">string</span><span class="sxs-lookup"><span data-stu-id="fe5ba-130">string</span></span> | <span data-ttu-id="fe5ba-131">Приложение/json.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-131">Application/json.</span></span> <span data-ttu-id="fe5ba-132">Обязательно указывать.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe5ba-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fe5ba-133">Request body</span></span>
<span data-ttu-id="fe5ba-134">В тексте запроса укажите представление объекта [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-134">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fe5ba-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe5ba-135">Response</span></span>
<span data-ttu-id="fe5ba-136">Успешно завершена, этот метод возвращает `202, Accepted` код ответа и объект [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-136">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe5ba-137">Пример</span><span class="sxs-lookup"><span data-stu-id="fe5ba-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe5ba-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="fe5ba-138">Request</span></span>
<span data-ttu-id="fe5ba-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="fe5ba-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="fe5ba-140">Response</span></span>
<span data-ttu-id="fe5ba-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-141">The following is an example of the response.</span></span> 

><span data-ttu-id="fe5ba-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fe5ba-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
