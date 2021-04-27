---
title: Создание educationSynchronizationProfile
description: 'Создайте запрос для нового профиля синхронизации школьных данных в клиенте. Запрос состояния, чтобы получить состояние профиля. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e55a24642f6b29ce280775f779f005fd76d4996c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043075"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="c6ee2-104">Создание educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="c6ee2-104">Create an educationSynchronizationProfile</span></span>

<span data-ttu-id="c6ee2-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6ee2-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6ee2-106">Создайте запрос для нового профиля синхронизации [школьных](../resources/educationsynchronizationprofile.md) данных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-106">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="c6ee2-107">[Запрос состояния,](educationsynchronizationprofilestatus-get.md) чтобы получить состояние профиля.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-107">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c6ee2-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ee2-108">Permissions</span></span>
<span data-ttu-id="c6ee2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c6ee2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c6ee2-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ee2-111">Permission type</span></span> | <span data-ttu-id="c6ee2-112">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c6ee2-112">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="c6ee2-113">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c6ee2-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c6ee2-114">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c6ee2-114">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="c6ee2-115">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c6ee2-115">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="c6ee2-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-116">Not supported.</span></span>|
|<span data-ttu-id="c6ee2-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c6ee2-117">Application</span></span>|<span data-ttu-id="c6ee2-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c6ee2-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c6ee2-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="c6ee2-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c6ee2-120">Request headers</span></span>
| <span data-ttu-id="c6ee2-121">Имя</span><span class="sxs-lookup"><span data-stu-id="c6ee2-121">Name</span></span>       | <span data-ttu-id="c6ee2-122">Тип</span><span class="sxs-lookup"><span data-stu-id="c6ee2-122">Type</span></span> | <span data-ttu-id="c6ee2-123">Описание</span><span class="sxs-lookup"><span data-stu-id="c6ee2-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c6ee2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6ee2-124">Authorization</span></span>  | <span data-ttu-id="c6ee2-125">string</span><span class="sxs-lookup"><span data-stu-id="c6ee2-125">string</span></span>  | <span data-ttu-id="c6ee2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6ee2-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6ee2-128">Content-Type</span></span> | <span data-ttu-id="c6ee2-129">string</span><span class="sxs-lookup"><span data-stu-id="c6ee2-129">string</span></span> | <span data-ttu-id="c6ee2-130">Application/json.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-130">Application/json.</span></span> <span data-ttu-id="c6ee2-131">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c6ee2-132">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c6ee2-132">Request body</span></span>
<span data-ttu-id="c6ee2-133">В теле запроса поставляем представление JSON объекта [educationSynchronizationProfile.](../resources/educationsynchronizationprofile.md)</span><span class="sxs-lookup"><span data-stu-id="c6ee2-133">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c6ee2-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ee2-134">Response</span></span>
<span data-ttu-id="c6ee2-135">В случае успеха этот метод возвращает код отклика и `202, Accepted` [объект educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-135">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c6ee2-136">Пример</span><span class="sxs-lookup"><span data-stu-id="c6ee2-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6ee2-137">Запрос</span><span class="sxs-lookup"><span data-stu-id="c6ee2-137">Request</span></span>
<span data-ttu-id="c6ee2-138">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-138">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c6ee2-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="c6ee2-139">Response</span></span>
<span data-ttu-id="c6ee2-140">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-140">The following is an example of the response.</span></span> 

><span data-ttu-id="c6ee2-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="c6ee2-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


