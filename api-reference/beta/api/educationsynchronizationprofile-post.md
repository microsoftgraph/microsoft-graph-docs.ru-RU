---
title: Создание Едукатионсинчронизатионпрофиле
description: 'Создайте запрос для нового профиля синхронизации данных School в клиенте. ЗаПросите состояние, чтобы получить состояние профиля. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: efc9b76405b57d0e47d645d0e7b00dc9425ba71b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457405"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="10314-104">Создание Едукатионсинчронизатионпрофиле</span><span class="sxs-lookup"><span data-stu-id="10314-104">Create an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10314-105">Создайте запрос для нового [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="10314-105">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="10314-106">[Запросите состояние](educationsynchronizationprofilestatus-get.md) , чтобы получить состояние профиля.</span><span class="sxs-lookup"><span data-stu-id="10314-106">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="10314-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10314-107">Permissions</span></span>
<span data-ttu-id="10314-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10314-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="10314-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10314-110">Permission type</span></span> | <span data-ttu-id="10314-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10314-111">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="10314-112">Делегированное (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10314-112">Delegated (work or school account)</span></span> | <span data-ttu-id="10314-113">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="10314-113">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="10314-114">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10314-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="10314-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10314-115">Not supported.</span></span>|
|<span data-ttu-id="10314-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10314-116">Application</span></span>|<span data-ttu-id="10314-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10314-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10314-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10314-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="10314-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10314-119">Request headers</span></span>
| <span data-ttu-id="10314-120">Имя</span><span class="sxs-lookup"><span data-stu-id="10314-120">Name</span></span>       | <span data-ttu-id="10314-121">Тип</span><span class="sxs-lookup"><span data-stu-id="10314-121">Type</span></span> | <span data-ttu-id="10314-122">Описание</span><span class="sxs-lookup"><span data-stu-id="10314-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="10314-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10314-123">Authorization</span></span>  | <span data-ttu-id="10314-124">string</span><span class="sxs-lookup"><span data-stu-id="10314-124">string</span></span>  | <span data-ttu-id="10314-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10314-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="10314-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="10314-127">Content-Type</span></span> | <span data-ttu-id="10314-128">string</span><span class="sxs-lookup"><span data-stu-id="10314-128">string</span></span> | <span data-ttu-id="10314-129">Приложение/JSON.</span><span class="sxs-lookup"><span data-stu-id="10314-129">Application/json.</span></span> <span data-ttu-id="10314-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="10314-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="10314-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10314-131">Request body</span></span>
<span data-ttu-id="10314-132">В тексте запроса добавьте представление объекта [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10314-132">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="10314-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="10314-133">Response</span></span>
<span data-ttu-id="10314-134">В случае успешного выполнения этот метод возвращает `202, Accepted` код отклика и объект [едукатионсинчронизатионпрофиле](../resources/educationsynchronizationprofile.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="10314-134">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10314-135">Пример</span><span class="sxs-lookup"><span data-stu-id="10314-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10314-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="10314-136">Request</span></span>
<span data-ttu-id="10314-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10314-137">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="10314-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="10314-138">Response</span></span>
<span data-ttu-id="10314-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="10314-139">The following is an example of the response.</span></span> 

><span data-ttu-id="10314-p106">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="10314-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofile-post.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
