---
title: Список educationSynchronizationProfiles
description: Получение коллекции школа данных синхронизации профилей в клиента.
ms.openlocfilehash: a303178a930f207aa92e7a49c769afbc06a7e1e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075670"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="bc3c5-103">Список educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="bc3c5-103">List educationSynchronizationProfiles</span></span>

> <span data-ttu-id="bc3c5-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc3c5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bc3c5-106">Получение коллекции данных school [синхронизации профилей](../resources/educationsynchronizationprofile.md) в клиентов.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-106">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="bc3c5-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc3c5-107">Permissions</span></span>
<span data-ttu-id="bc3c5-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc3c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bc3c5-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc3c5-110">Permission type</span></span> | <span data-ttu-id="bc3c5-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc3c5-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="bc3c5-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc3c5-112">Delegated (work or school account)</span></span> | <span data-ttu-id="bc3c5-113">EduAdministration.Read EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bc3c5-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="bc3c5-114">Делегированные (личная учетная запись Майкрософт</span><span class="sxs-lookup"><span data-stu-id="bc3c5-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="bc3c5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-115">Not supported.</span></span>|
|<span data-ttu-id="bc3c5-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc3c5-116">Application</span></span>|<span data-ttu-id="bc3c5-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bc3c5-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc3c5-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bc3c5-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bc3c5-119">Optional query parameters</span></span>
<span data-ttu-id="bc3c5-120">Этот метод поддерживает следующие [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа: $filter, $orderby, $top, $skip и $count.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-120">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bc3c5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bc3c5-121">Request headers</span></span>
| <span data-ttu-id="bc3c5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bc3c5-122">Name</span></span>       | <span data-ttu-id="bc3c5-123">Тип</span><span class="sxs-lookup"><span data-stu-id="bc3c5-123">Type</span></span> | <span data-ttu-id="bc3c5-124">Описание</span><span class="sxs-lookup"><span data-stu-id="bc3c5-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="bc3c5-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc3c5-125">Authorization</span></span>  | <span data-ttu-id="bc3c5-126">string</span><span class="sxs-lookup"><span data-stu-id="bc3c5-126">string</span></span>  | <span data-ttu-id="bc3c5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bc3c5-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="bc3c5-129">Request body</span></span>
<span data-ttu-id="bc3c5-130">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-130">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="bc3c5-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc3c5-131">Response</span></span>
<span data-ttu-id="bc3c5-132">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-132">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bc3c5-133">Пример</span><span class="sxs-lookup"><span data-stu-id="bc3c5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bc3c5-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="bc3c5-134">Request</span></span>
<span data-ttu-id="bc3c5-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "list_synchronizationProfile"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```

##### <a name="response"></a><span data-ttu-id="bc3c5-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="bc3c5-136">Response</span></span>
<span data-ttu-id="bc3c5-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-137">The following is an example of the response.</span></span> 

><span data-ttu-id="bc3c5-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="bc3c5-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "#microsoft.graph.educationSynchronizationProfile",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 3296

{
    "value": [
    {
        "displayName": "Test Profile",
        "state": "provisioned",
        "id": "15e9b9fa-de85-492e-aa44-550c40de626e",
        "dataProvider": {
            "@odata.type": "#microsoft.graph.educationCsvDataProvider",
            "customizations": {
                "school": {
                    "optionalPropertiesToSync": [
                        "School NCES_ID",
                        "State ID",
                        "GradeLow",
                        "GradeHigh",
                        "Principal Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "section": {
                    "optionalPropertiesToSync": [],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "student": {
                    "optionalPropertiesToSync": [
                        "State ID",
                        "Email",
                        "Middle Name"
                    ],
                    "synchronizationStartDate": "0001-01-01T00:00:00Z",
                    "isSyncDeferred": false,
                    "allowDisplayNameUpdate": false
                },
                "teacher": {
                    "optionalPropertiesToSync": [
                        "Teacher Number",
                        "Middle Name"
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
  ]
}
```