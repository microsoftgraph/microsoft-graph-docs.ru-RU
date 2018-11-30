---
title: Создание educationSynchronizationProfile
description: 'Создание запроса для школа данных синхронизации профиля в клиентов. Запрос состояния, чтобы получить сведения о состоянии профиля. '
ms.openlocfilehash: 0d2c4126ab92e376919ee0b69378754828a924a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077594"
---
# <a name="create-an-educationsynchronizationprofile"></a><span data-ttu-id="5472a-104">Создание educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="5472a-104">Create an educationSynchronizationProfile</span></span>

> <span data-ttu-id="5472a-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="5472a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5472a-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5472a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5472a-107">Создание запроса для нового данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="5472a-107">Create a request for a new school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="5472a-108">[Запрос состояния](educationsynchronizationprofilestatus-get.md) , чтобы получить сведения о состоянии профиля.</span><span class="sxs-lookup"><span data-stu-id="5472a-108">[Query the status](educationsynchronizationprofilestatus-get.md) to get the status of the profile.</span></span> 

## <a name="permissions"></a><span data-ttu-id="5472a-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5472a-109">Permissions</span></span>
<span data-ttu-id="5472a-p104">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5472a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5472a-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5472a-112">Permission type</span></span> | <span data-ttu-id="5472a-113">Permissions</span><span class="sxs-lookup"><span data-stu-id="5472a-113">Permissions</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5472a-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5472a-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5472a-115">EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5472a-115">EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5472a-116">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="5472a-116">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5472a-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5472a-117">Not supported.</span></span>|
|<span data-ttu-id="5472a-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5472a-118">Application</span></span>|<span data-ttu-id="5472a-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5472a-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5472a-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5472a-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles
```

## <a name="request-headers"></a><span data-ttu-id="5472a-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5472a-121">Request headers</span></span>
| <span data-ttu-id="5472a-122">Имя</span><span class="sxs-lookup"><span data-stu-id="5472a-122">Name</span></span>       | <span data-ttu-id="5472a-123">Тип</span><span class="sxs-lookup"><span data-stu-id="5472a-123">Type</span></span> | <span data-ttu-id="5472a-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5472a-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5472a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5472a-125">Authorization</span></span>  | <span data-ttu-id="5472a-126">string</span><span class="sxs-lookup"><span data-stu-id="5472a-126">string</span></span>  | <span data-ttu-id="5472a-p105">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5472a-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5472a-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5472a-129">Content-Type</span></span> | <span data-ttu-id="5472a-130">string</span><span class="sxs-lookup"><span data-stu-id="5472a-130">string</span></span> | <span data-ttu-id="5472a-131">Приложение/json.</span><span class="sxs-lookup"><span data-stu-id="5472a-131">Application/json.</span></span> <span data-ttu-id="5472a-132">Обязательный атрибут.</span><span class="sxs-lookup"><span data-stu-id="5472a-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5472a-133">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5472a-133">Request body</span></span>
<span data-ttu-id="5472a-134">В тексте запроса укажите представление объекта [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) с JSON.</span><span class="sxs-lookup"><span data-stu-id="5472a-134">In the request body, supply a JSON representation of the [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5472a-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="5472a-135">Response</span></span>
<span data-ttu-id="5472a-136">Успешно завершена, этот метод возвращает `202, Accepted` код ответа и объект [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="5472a-136">If successful, this method returns a `202, Accepted` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5472a-137">Пример</span><span class="sxs-lookup"><span data-stu-id="5472a-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5472a-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="5472a-138">Request</span></span>
<span data-ttu-id="5472a-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5472a-139">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="5472a-140">Ответ</span><span class="sxs-lookup"><span data-stu-id="5472a-140">Response</span></span>
<span data-ttu-id="5472a-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5472a-141">The following is an example of the response.</span></span> 

><span data-ttu-id="5472a-p107">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="5472a-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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