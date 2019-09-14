---
title: Создание Едукатионсинчронизатионпрофиле
description: 'Создайте запрос для нового профиля синхронизации данных School в клиенте. Запросите состояние, чтобы получить состояние профиля. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 314cb71f5f3ebf135cab0ef3bf9cc9afff9eb730
ms.sourcegitcommit: c739cbfab42181adfcda409ca12514ab7f4832b1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/14/2019
ms.locfileid: "36982882"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="bac14-104">Создание Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="bac14-104">Create an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bac14-105">Создайте запрос для нового [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="bac14-105">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="bac14-106">[Запросите состояние](educationsynchronizationprofilestatus-get.md) , чтобы получить состояние профиля.</span><span class="sxs-lookup"><span data-stu-id="bac14-106">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bac14-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bac14-107">Permissions</span></span>
<span data-ttu-id="bac14-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bac14-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bac14-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bac14-110">Permission type</span></span> | <span data-ttu-id="bac14-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bac14-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="bac14-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bac14-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bac14-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bac14-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="bac14-114">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bac14-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bac14-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bac14-115">Not supported.</span></span>|
|<span data-ttu-id="bac14-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bac14-116">Application</span></span>|<span data-ttu-id="bac14-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bac14-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bac14-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bac14-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="bac14-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bac14-119">Request headers</span></span>
| <span data-ttu-id="bac14-120">Имя</span><span class="sxs-lookup"><span data-stu-id="bac14-120">Name</span></span>       | <span data-ttu-id="bac14-121">Тип</span><span class="sxs-lookup"><span data-stu-id="bac14-121">Type</span></span> | <span data-ttu-id="bac14-122">Описание</span><span class="sxs-lookup"><span data-stu-id="bac14-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bac14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bac14-123">Authorization</span></span>  | <span data-ttu-id="bac14-124">string</span><span class="sxs-lookup"><span data-stu-id="bac14-124">string</span></span>  | <span data-ttu-id="bac14-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bac14-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bac14-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bac14-127">Content-Type</span></span> | <span data-ttu-id="bac14-128">string</span><span class="sxs-lookup"><span data-stu-id="bac14-128">string</span></span> | <span data-ttu-id="bac14-129">Приложение/JSON.</span><span class="sxs-lookup"><span data-stu-id="bac14-129">Application/json.</span></span> <span data-ttu-id="bac14-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="bac14-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bac14-131">Основной текст запросов</span><span class="sxs-lookup"><span data-stu-id="bac14-131">Request body</span></span>
<span data-ttu-id="bac14-132">В тексте запроса добавьте представление объекта [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bac14-132">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="bac14-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bac14-133">Response</span></span>
<span data-ttu-id="bac14-134">В случае успешного выполнения этот метод возвращает `202, Accepted` код отклика и объект [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bac14-134">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bac14-135">Пример</span><span class="sxs-lookup"><span data-stu-id="bac14-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bac14-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="bac14-136">Request</span></span>
<span data-ttu-id="bac14-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bac14-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="bac14-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="bac14-138">Response</span></span>
<span data-ttu-id="bac14-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bac14-139">The following is an example of the response.</span></span> 

><span data-ttu-id="bac14-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bac14-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
