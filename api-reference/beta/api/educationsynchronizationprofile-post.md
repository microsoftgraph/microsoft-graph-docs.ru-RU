---
title: Создание educationSynchronizationProfile
description: 'Создание запроса для школа данных синхронизации профиля в клиентов. Запрос состояния, чтобы получить сведения о состоянии профиля. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9d471766a8492e03809d05d6d0366c8e44d59015
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27915762"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="b19be-104">Создание educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="b19be-104">Create an educationSynchronizationProfile</span></span>

> <span data-ttu-id="b19be-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b19be-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b19be-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b19be-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b19be-107">Создание запроса для нового данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="b19be-107">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="b19be-108">[Запрос состояния](educationsynchronizationprofilestatus-get.md) , чтобы получить сведения о состоянии профиля.</span><span class="sxs-lookup"><span data-stu-id="b19be-108">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b19be-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b19be-109">Permissions</span></span>
<span data-ttu-id="b19be-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b19be-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b19be-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b19be-112">Permission type</span></span> | <span data-ttu-id="b19be-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="b19be-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="b19be-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b19be-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b19be-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b19be-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="b19be-116">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="b19be-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="b19be-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b19be-117">Not supported.</span></span>|
|<span data-ttu-id="b19be-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b19be-118">Application</span></span>|<span data-ttu-id="b19be-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b19be-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b19be-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b19be-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="b19be-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b19be-121">Request headers</span></span>
| <span data-ttu-id="b19be-122">Имя</span><span class="sxs-lookup"><span data-stu-id="b19be-122">Name</span></span>       | <span data-ttu-id="b19be-123">Тип</span><span class="sxs-lookup"><span data-stu-id="b19be-123">Type</span></span> | <span data-ttu-id="b19be-124">Описание</span><span class="sxs-lookup"><span data-stu-id="b19be-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b19be-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="b19be-125">Authorization</span></span>  | <span data-ttu-id="b19be-126">string</span><span class="sxs-lookup"><span data-stu-id="b19be-126">string</span></span>  | <span data-ttu-id="b19be-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b19be-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b19be-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b19be-129">Content-Type</span></span> | <span data-ttu-id="b19be-130">string</span><span class="sxs-lookup"><span data-stu-id="b19be-130">string</span></span> | <span data-ttu-id="b19be-131">Приложение/json.</span><span class="sxs-lookup"><span data-stu-id="b19be-131">Application/json.</span></span> <span data-ttu-id="b19be-132">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="b19be-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b19be-133">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b19be-133">Request body</span></span>
<span data-ttu-id="b19be-134">В тексте запроса укажите представление объекта [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="b19be-134">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b19be-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="b19be-135">Response</span></span>
<span data-ttu-id="b19be-136">Успешно завершена, этот метод возвращает `202, Accepted` код ответа и объект [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="b19be-136">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b19be-137">Пример</span><span class="sxs-lookup"><span data-stu-id="b19be-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b19be-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="b19be-138">Request</span></span>
<span data-ttu-id="b19be-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b19be-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="b19be-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="b19be-140">Response</span></span>
<span data-ttu-id="b19be-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b19be-141">The following is an example of the response.</span></span> 

><span data-ttu-id="b19be-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b19be-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
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
