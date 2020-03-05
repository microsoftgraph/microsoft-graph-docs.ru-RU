---
title: Получение Едукатионсинчронизатионеррорс
description: 'Получение ошибок, возникших во время проверки, и/или во время синхронизации определенного профиля синхронизации данных School в клиенте. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 81da0a081976e97254b541c0d4d07e13ed51c854
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42424612"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="969b5-103">Получение Едукатионсинчронизатионеррорс</span><span class="sxs-lookup"><span data-stu-id="969b5-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="969b5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="969b5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="969b5-105">Получение ошибок, возникших во время проверки, и/или во время синхронизации определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="969b5-105">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="969b5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="969b5-106">Permissions</span></span>
<span data-ttu-id="969b5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="969b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="969b5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="969b5-109">Permission type</span></span> | <span data-ttu-id="969b5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="969b5-110">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="969b5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="969b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="969b5-112">Едуадминистратион. Read, Едуадминистратион. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="969b5-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="969b5-113">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="969b5-113">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="969b5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="969b5-114">Not supported.</span></span>|
|<span data-ttu-id="969b5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="969b5-115">Application</span></span>| <span data-ttu-id="969b5-116">Едуадминистратион. Read. ALL, Едуадминистратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="969b5-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="969b5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="969b5-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="969b5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="969b5-118">Optional query parameters</span></span>
<span data-ttu-id="969b5-119">Этот метод поддерживает следующие [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика: $filter, $orderby, $top, $skip и $Count.</span><span class="sxs-lookup"><span data-stu-id="969b5-119">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="969b5-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="969b5-120">Request headers</span></span>
| <span data-ttu-id="969b5-121">Имя</span><span class="sxs-lookup"><span data-stu-id="969b5-121">Name</span></span>       | <span data-ttu-id="969b5-122">Тип</span><span class="sxs-lookup"><span data-stu-id="969b5-122">Type</span></span> | <span data-ttu-id="969b5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="969b5-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="969b5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="969b5-124">Authorization</span></span>  | <span data-ttu-id="969b5-125">string</span><span class="sxs-lookup"><span data-stu-id="969b5-125">string</span></span>  | <span data-ttu-id="969b5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="969b5-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="969b5-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="969b5-128">Request body</span></span>
<span data-ttu-id="969b5-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="969b5-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="969b5-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="969b5-130">Response</span></span>
<span data-ttu-id="969b5-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Error синхронизации](../resources/educationsynchronizationerror.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="969b5-131">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="969b5-132">Пример</span><span class="sxs-lookup"><span data-stu-id="969b5-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="969b5-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="969b5-133">Request</span></span>
<span data-ttu-id="969b5-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="969b5-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="969b5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="969b5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="c"></a>[<span data-ttu-id="969b5-136">C#</span><span class="sxs-lookup"><span data-stu-id="969b5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="969b5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="969b5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="969b5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="969b5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="969b5-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="969b5-139">Response</span></span>
<span data-ttu-id="969b5-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="969b5-140">The following is an example of the response.</span></span> 

><span data-ttu-id="969b5-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="969b5-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationError",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1568

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles/{id}/errors",
    "@odata.count": 14,
    "value": [
        {
            "entryType": "Student",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
            "joiningValue": "richard.2wilson@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:45Z",
            "reportableIdentifier": "richard.2wilson"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "alberto2.dorsey@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "alberto2.dorsey"
        },
        {
            "entryType": "Teacher",
            "errorCode": "UnsynchronizableChange",
            "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
            "joiningValue": "madeline2.bullock@testschool.edu",
            "recordedDateTime": "2017-07-05T00:52:57Z",
            "reportableIdentifier": "madeline2.bullock"
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
