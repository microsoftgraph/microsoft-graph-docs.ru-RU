---
title: Get an educationSynchronizationProfile
description: Извлечение профиля синхронизации школьных данных в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1810fe299b62a52c2b56d9fccb2f312638beff06
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52043117"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="71793-103">Get an educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="71793-103">Get an educationSynchronizationProfile</span></span>

<span data-ttu-id="71793-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71793-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71793-105">Извлечение профиля [синхронизации школьных данных](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="71793-105">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="71793-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71793-106">Permissions</span></span>
<span data-ttu-id="71793-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71793-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71793-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71793-109">Permission type</span></span> | <span data-ttu-id="71793-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71793-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="71793-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71793-111">Delegated (work or school account)</span></span> | <span data-ttu-id="71793-112">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71793-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="71793-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71793-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="71793-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71793-114">Not supported.</span></span>|
|<span data-ttu-id="71793-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71793-115">Application</span></span>| <span data-ttu-id="71793-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71793-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71793-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71793-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="71793-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71793-118">Request headers</span></span>
| <span data-ttu-id="71793-119">Имя</span><span class="sxs-lookup"><span data-stu-id="71793-119">Name</span></span>       | <span data-ttu-id="71793-120">Тип</span><span class="sxs-lookup"><span data-stu-id="71793-120">Type</span></span> | <span data-ttu-id="71793-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71793-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="71793-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71793-122">Authorization</span></span>  | <span data-ttu-id="71793-123">string</span><span class="sxs-lookup"><span data-stu-id="71793-123">string</span></span>  | <span data-ttu-id="71793-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71793-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71793-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71793-126">Request body</span></span>
<span data-ttu-id="71793-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71793-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="71793-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="71793-128">Response</span></span>
<span data-ttu-id="71793-129">В случае успеха этот метод возвращает код отклика и `200 OK` [объект educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71793-129">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71793-130">Пример</span><span class="sxs-lookup"><span data-stu-id="71793-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71793-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="71793-131">Request</span></span>
<span data-ttu-id="71793-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71793-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71793-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="71793-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="71793-134">C#</span><span class="sxs-lookup"><span data-stu-id="71793-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71793-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71793-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71793-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71793-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71793-137">Java</span><span class="sxs-lookup"><span data-stu-id="71793-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71793-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="71793-138">Response</span></span>
<span data-ttu-id="71793-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="71793-139">The following is an example of the response.</span></span> 

><span data-ttu-id="71793-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="71793-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSynchronizationProfile",
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
    "licensesToAssign": 
         [
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


