---
title: Получение educationSynchronizationProfile
description: Извлечение профиля синхронизации данных school в клиентов на основе идентификатора.
ms.openlocfilehash: a62b938f3177f06a02a8a5ad1190d72b3f27dfd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074682"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="27831-103">Получение educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="27831-103">Get an educationSynchronizationProfile</span></span>

> <span data-ttu-id="27831-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="27831-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27831-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27831-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27831-106">Получение в школе данных [синхронизации профилей](../resources/educationsynchronizationprofile.md) на основе идентификатора клиента.</span><span class="sxs-lookup"><span data-stu-id="27831-106">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="27831-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="27831-107">Permissions</span></span>
<span data-ttu-id="27831-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="27831-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="27831-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="27831-110">Permission type</span></span> | <span data-ttu-id="27831-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="27831-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="27831-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="27831-112">Delegated (work or school account)</span></span> | <span data-ttu-id="27831-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="27831-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="27831-114">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="27831-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="27831-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="27831-115">Not supported.</span></span>|
|<span data-ttu-id="27831-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="27831-116">Application</span></span>| <span data-ttu-id="27831-117">EduAdministration.Read.All EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27831-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="27831-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="27831-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="27831-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="27831-119">Request headers</span></span>
| <span data-ttu-id="27831-120">Имя</span><span class="sxs-lookup"><span data-stu-id="27831-120">Name</span></span>       | <span data-ttu-id="27831-121">Тип</span><span class="sxs-lookup"><span data-stu-id="27831-121">Type</span></span> | <span data-ttu-id="27831-122">Описание</span><span class="sxs-lookup"><span data-stu-id="27831-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="27831-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27831-123">Authorization</span></span>  | <span data-ttu-id="27831-124">string</span><span class="sxs-lookup"><span data-stu-id="27831-124">string</span></span>  | <span data-ttu-id="27831-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="27831-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="27831-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="27831-127">Request body</span></span>
<span data-ttu-id="27831-128">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="27831-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="27831-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="27831-129">Response</span></span>
<span data-ttu-id="27831-130">Успешно завершена, этот метод возвращает `200 OK` код ответа и объект [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="27831-130">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27831-131">Пример</span><span class="sxs-lookup"><span data-stu-id="27831-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="27831-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="27831-132">Request</span></span>
<span data-ttu-id="27831-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="27831-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationSynchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```

##### <a name="response"></a><span data-ttu-id="27831-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="27831-134">Response</span></span>
<span data-ttu-id="27831-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="27831-135">The following is an example of the response.</span></span> 

><span data-ttu-id="27831-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="27831-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 2487

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/$entity",
    "displayName": "Test Profile",
    "state": "provisioned",
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
    "licensesToAssign": 
         [
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
