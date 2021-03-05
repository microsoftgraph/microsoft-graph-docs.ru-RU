---
title: List educationSynchronizationProfiles
description: Извлечение коллекции профилей синхронизации школьных данных в клиенте.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: ad8249c01bee946deca4e380eb359903f5be7b6f
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470518"
---
# <a name="list-educationsynchronizationprofiles"></a><span data-ttu-id="073e5-103">List educationSynchronizationProfiles</span><span class="sxs-lookup"><span data-stu-id="073e5-103">List educationSynchronizationProfiles</span></span>

<span data-ttu-id="073e5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="073e5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="073e5-105">Извлечение коллекции профилей [синхронизации школьных данных](../resources/educationsynchronizationprofile.md) в клиенте.</span><span class="sxs-lookup"><span data-stu-id="073e5-105">Retrieve the collection of school data [synchronization profiles](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="073e5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="073e5-106">Permissions</span></span>
<span data-ttu-id="073e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="073e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="073e5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="073e5-109">Permission type</span></span> | <span data-ttu-id="073e5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="073e5-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="073e5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="073e5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="073e5-112">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="073e5-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="073e5-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="073e5-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="073e5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="073e5-114">Not supported.</span></span>|
|<span data-ttu-id="073e5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="073e5-115">Application</span></span>|<span data-ttu-id="073e5-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="073e5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="073e5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="073e5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="073e5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="073e5-118">Optional query parameters</span></span>
<span data-ttu-id="073e5-119">Этот метод поддерживает следующие параметры запроса [OData](/graph/query-parameters) для настройки ответа: $filter, $orderby, $top, $skip и $count.</span><span class="sxs-lookup"><span data-stu-id="073e5-119">This method supports the following [OData Query Parameters](/graph/query-parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="073e5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="073e5-120">Request headers</span></span>
| <span data-ttu-id="073e5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="073e5-121">Name</span></span>       | <span data-ttu-id="073e5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="073e5-122">Type</span></span> | <span data-ttu-id="073e5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="073e5-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="073e5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="073e5-124">Authorization</span></span>  | <span data-ttu-id="073e5-125">string</span><span class="sxs-lookup"><span data-stu-id="073e5-125">string</span></span>  | <span data-ttu-id="073e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="073e5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="073e5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="073e5-128">Request body</span></span>
<span data-ttu-id="073e5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="073e5-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="073e5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="073e5-130">Response</span></span>
<span data-ttu-id="073e5-131">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="073e5-131">If successful, this method returns a `200 OK` response code and a collection of [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="073e5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="073e5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="073e5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="073e5-133">Request</span></span>
<span data-ttu-id="073e5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="073e5-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="073e5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="073e5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_synchronizationProfile"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles
```
# <a name="c"></a>[<span data-ttu-id="073e5-136">C#</span><span class="sxs-lookup"><span data-stu-id="073e5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-synchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="073e5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="073e5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-synchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="073e5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="073e5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-synchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="073e5-139">Java</span><span class="sxs-lookup"><span data-stu-id="073e5-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-synchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="073e5-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="073e5-140">Response</span></span>
<span data-ttu-id="073e5-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="073e5-141">The following is an example of the response.</span></span> 

><span data-ttu-id="073e5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="073e5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
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
            "@odata.type": "microsoft.graph.educationCsvDataProvider",
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
  ]
}
```
