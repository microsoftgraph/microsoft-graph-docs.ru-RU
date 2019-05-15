---
title: Получение Едукатионсинчронизатионеррорс
description: 'Получение ошибок, возникших во время проверки, и/или во время синхронизации определенного профиля синхронизации данных School в клиенте. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 84c0139e950274de6d8d625d00787784b52661bb
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/13/2019
ms.locfileid: "33960874"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="a4bcc-103">Получение Едукатионсинчронизатионеррорс</span><span class="sxs-lookup"><span data-stu-id="a4bcc-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="a4bcc-104">Получение ошибок, возникших во время проверки, и/или во время синхронизации определенного [профиля синхронизации](../resources/educationsynchronizationprofile.md) данных School в клиенте.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-104">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> 

## <a name="permissions"></a><span data-ttu-id="a4bcc-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a4bcc-105">Permissions</span></span>
<span data-ttu-id="a4bcc-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a4bcc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a4bcc-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a4bcc-108">Permission type</span></span> | <span data-ttu-id="a4bcc-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a4bcc-109">Permissions (from least to most privileged)</span></span> |
|:-----------|:------|
| <span data-ttu-id="a4bcc-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a4bcc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a4bcc-111">Едуадминистратион. Read, Едуадминистратион. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a4bcc-111">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="a4bcc-112">Делегированная учетная запись (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a4bcc-112">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="a4bcc-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-113">Not supported.</span></span>|
|<span data-ttu-id="a4bcc-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a4bcc-114">Application</span></span>| <span data-ttu-id="a4bcc-115">Едуадминистратион. Read. ALL, Едуадминистратион. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="a4bcc-115">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a4bcc-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a4bcc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/errors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a4bcc-117">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a4bcc-117">Optional query parameters</span></span>
<span data-ttu-id="a4bcc-118">Этот метод поддерживает следующие [Параметры запроса OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки отклика: $filter, $orderby, $top, $skip и $Count.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-118">This method supports the following [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response: $filter, $orderby, $top, $skip, and $count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a4bcc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a4bcc-119">Request headers</span></span>
| <span data-ttu-id="a4bcc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a4bcc-120">Name</span></span>       | <span data-ttu-id="a4bcc-121">Тип</span><span class="sxs-lookup"><span data-stu-id="a4bcc-121">Type</span></span> | <span data-ttu-id="a4bcc-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a4bcc-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="a4bcc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a4bcc-123">Authorization</span></span>  | <span data-ttu-id="a4bcc-124">string</span><span class="sxs-lookup"><span data-stu-id="a4bcc-124">string</span></span>  | <span data-ttu-id="a4bcc-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a4bcc-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a4bcc-127">Request body</span></span>
<span data-ttu-id="a4bcc-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a4bcc-129">Ответ</span><span class="sxs-lookup"><span data-stu-id="a4bcc-129">Response</span></span>
<span data-ttu-id="a4bcc-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [Error синхронизации](../resources/educationsynchronizationerror.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-130">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a4bcc-131">Пример</span><span class="sxs-lookup"><span data-stu-id="a4bcc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a4bcc-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="a4bcc-132">Request</span></span>
<span data-ttu-id="a4bcc-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```

##### <a name="response"></a><span data-ttu-id="a4bcc-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="a4bcc-134">Response</span></span>
<span data-ttu-id="a4bcc-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-135">The following is an example of the response.</span></span> 

><span data-ttu-id="a4bcc-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a4bcc-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/errors",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a4bcc-138">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="a4bcc-138">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a4bcc-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="a4bcc-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_error-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="a4bcc-140">C#</span><span class="sxs-lookup"><span data-stu-id="a4bcc-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_error-Cs-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationerrors-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationerrors-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
