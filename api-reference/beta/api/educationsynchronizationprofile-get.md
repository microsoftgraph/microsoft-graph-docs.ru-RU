---
title: Get an educationSynchronizationProfile
description: Извлечение профиля синхронизации школьных данных в клиенте на основе идентификатора.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b3dd16ba86e455e63f21132cc67a1c33b055a1d6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470444"
---
# <a name="get-an-educationsynchronizationprofile"></a><span data-ttu-id="71ed7-103">Get an educationSynchronizationProfile</span><span class="sxs-lookup"><span data-stu-id="71ed7-103">Get an educationSynchronizationProfile</span></span>

<span data-ttu-id="71ed7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71ed7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71ed7-105">Извлечение профиля [синхронизации школьных данных](../resources/educationsynchronizationprofile.md) в клиенте на основе идентификатора.</span><span class="sxs-lookup"><span data-stu-id="71ed7-105">Retrieve a school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant based on the identifier.</span></span>

## <a name="permissions"></a><span data-ttu-id="71ed7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71ed7-106">Permissions</span></span>
<span data-ttu-id="71ed7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71ed7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="71ed7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71ed7-109">Permission type</span></span> | <span data-ttu-id="71ed7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71ed7-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="71ed7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71ed7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="71ed7-112">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71ed7-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="71ed7-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71ed7-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="71ed7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71ed7-114">Not supported.</span></span>|
|<span data-ttu-id="71ed7-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="71ed7-115">Application</span></span>| <span data-ttu-id="71ed7-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71ed7-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71ed7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71ed7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}
```

## <a name="request-headers"></a><span data-ttu-id="71ed7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71ed7-118">Request headers</span></span>
| <span data-ttu-id="71ed7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="71ed7-119">Name</span></span>       | <span data-ttu-id="71ed7-120">Тип</span><span class="sxs-lookup"><span data-stu-id="71ed7-120">Type</span></span> | <span data-ttu-id="71ed7-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71ed7-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="71ed7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="71ed7-122">Authorization</span></span>  | <span data-ttu-id="71ed7-123">string</span><span class="sxs-lookup"><span data-stu-id="71ed7-123">string</span></span>  | <span data-ttu-id="71ed7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71ed7-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="71ed7-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71ed7-126">Request body</span></span>
<span data-ttu-id="71ed7-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71ed7-127">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="71ed7-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ed7-128">Response</span></span>
<span data-ttu-id="71ed7-129">В случае успеха этот метод возвращает код отклика и `200 OK` [объект educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="71ed7-129">If successful, this method returns a `200 OK` response code and an [educationSynchronizationProfile](../resources/educationsynchronizationprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71ed7-130">Пример</span><span class="sxs-lookup"><span data-stu-id="71ed7-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71ed7-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="71ed7-131">Request</span></span>
<span data-ttu-id="71ed7-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71ed7-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71ed7-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="71ed7-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}
```
# <a name="c"></a>[<span data-ttu-id="71ed7-134">C#</span><span class="sxs-lookup"><span data-stu-id="71ed7-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="71ed7-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71ed7-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71ed7-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71ed7-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71ed7-137">Java</span><span class="sxs-lookup"><span data-stu-id="71ed7-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="71ed7-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="71ed7-138">Response</span></span>
<span data-ttu-id="71ed7-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="71ed7-139">The following is an example of the response.</span></span> 

><span data-ttu-id="71ed7-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="71ed7-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


