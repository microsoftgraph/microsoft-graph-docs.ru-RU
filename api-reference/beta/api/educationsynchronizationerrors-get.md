---
title: Get educationSynchronizationErrors
description: 'Получите ошибки, созданные во время проверки и/или при синхронизации определенного профиля синхронизации школьных данных в клиенте. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a3b2e0b9018d3a6d34073530f8bd846a4d6df64c
ms.sourcegitcommit: ceb192c3a41feb74cd720ddf2f0119c48bf1189b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/09/2021
ms.locfileid: "50574274"
---
# <a name="get-educationsynchronizationerrors"></a><span data-ttu-id="0ea61-103">Get educationSynchronizationErrors</span><span class="sxs-lookup"><span data-stu-id="0ea61-103">Get educationSynchronizationErrors</span></span>

<span data-ttu-id="0ea61-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0ea61-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0ea61-105">Получите ошибки, созданные во время проверки и/или при синхронизации определенного профиля синхронизации школьных данных [в](../resources/educationsynchronizationprofile.md) клиенте.</span><span class="sxs-lookup"><span data-stu-id="0ea61-105">Get the errors generated during validation and/or during a sync of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea61-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea61-106">Permissions</span></span>

<span data-ttu-id="0ea61-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ea61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0ea61-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ea61-109">Permission type</span></span>                       | <span data-ttu-id="0ea61-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ea61-110">Permissions (from least to most privileged)</span></span>                 |
| :------------------------------------ | :---------------------------------------------------------- |
| <span data-ttu-id="0ea61-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ea61-111">Delegated (work or school account)</span></span>    | <span data-ttu-id="0ea61-112">EduAdministration.Read, EduAdministration.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0ea61-112">EduAdministration.Read, EduAdministration.ReadWrite</span></span>         |
| <span data-ttu-id="0ea61-113">Делегированная (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ea61-113">Delegated (personal Microsoft account</span></span> | <span data-ttu-id="0ea61-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ea61-114">Not supported.</span></span>                                              |
| <span data-ttu-id="0ea61-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0ea61-115">Application</span></span>                           | <span data-ttu-id="0ea61-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ea61-116">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ea61-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ea61-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /education/synchronizationProfiles/{id}/errors
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ea61-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0ea61-118">Optional query parameters</span></span>

<span data-ttu-id="0ea61-119">Этот метод поддерживает следующие параметры запроса [OData](/graph/query-parameters) для настройки ответа: $filter, $orderby, $top, $skip и \$ подсчета.</span><span class="sxs-lookup"><span data-stu-id="0ea61-119">This method supports the following [OData Query Parameters](/graph/query-parameters) to help customize the response: $filter, $orderby, $top, $skip, and \$count.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ea61-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ea61-120">Request headers</span></span>

| <span data-ttu-id="0ea61-121">Имя</span><span class="sxs-lookup"><span data-stu-id="0ea61-121">Name</span></span>          | <span data-ttu-id="0ea61-122">Тип</span><span class="sxs-lookup"><span data-stu-id="0ea61-122">Type</span></span>   | <span data-ttu-id="0ea61-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0ea61-123">Description</span></span>               |
| :------------ | :----- | :------------------------ |
| <span data-ttu-id="0ea61-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea61-124">Authorization</span></span> | <span data-ttu-id="0ea61-125">string</span><span class="sxs-lookup"><span data-stu-id="0ea61-125">string</span></span> | <span data-ttu-id="0ea61-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0ea61-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0ea61-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ea61-128">Request body</span></span>

<span data-ttu-id="0ea61-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0ea61-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea61-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ea61-130">Response</span></span>

<span data-ttu-id="0ea61-131">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов ошибки синхронизации `200 OK` в тексте [](../resources/educationsynchronizationerror.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="0ea61-131">If successful, this method returns a `200 OK` response code and a collection of [synchronization error](../resources/educationsynchronizationerror.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ea61-132">Пример</span><span class="sxs-lookup"><span data-stu-id="0ea61-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0ea61-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ea61-133">Request</span></span>

<span data-ttu-id="0ea61-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ea61-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0ea61-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0ea61-135">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_error"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/errors
```
# <a name="c"></a>[<span data-ttu-id="0ea61-136">C#</span><span class="sxs-lookup"><span data-stu-id="0ea61-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-educationsynchronizationprofile-error-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0ea61-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0ea61-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-educationsynchronizationprofile-error-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0ea61-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0ea61-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-educationsynchronizationprofile-error-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0ea61-139">Java</span><span class="sxs-lookup"><span data-stu-id="0ea61-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-educationsynchronizationprofile-error-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0ea61-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ea61-140">Response</span></span>

<span data-ttu-id="0ea61-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ea61-141">The following is an example of the response.</span></span>

> <span data-ttu-id="0ea61-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0ea61-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "id": "92797B7C-02C3-4326-8ACC-E81C78753831",
      "entryType": "Student",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Student cannot be updated as no matching entry in Active Directory was found for Student.  Verify the identity matching criteria for the profile.",
      "joiningValue": "richard.2wilson@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:45Z",
      "reportableIdentifier": "richard.2wilson"
    },
    {
      "id": "94C1EB0E-8339-4EF4-8CB2-EB15C6228CE1",
      "entryType": "Teacher",
      "errorCode": "UnsynchronizableChange",
      "errorMessage": "Teacher cannot be updated as no matching entry in Active Directory was found for Teacher.  Verify the identity matching criteria for the profile.",
      "joiningValue": "alberto2.dorsey@testschool.edu",
      "recordedDateTime": "2017-07-05T00:52:57Z",
      "reportableIdentifier": "alberto2.dorsey"
    },
    {
      "id": "98A82052-7716-49E9-90CC-C6FF406FC8E5",
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
