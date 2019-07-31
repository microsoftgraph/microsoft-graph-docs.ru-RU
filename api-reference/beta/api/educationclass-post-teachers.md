---
title: Добавление преподавателя
description: Добавление преподавателя в класс.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dde692dfd76f484dbaadcb4b0086e31618d3e80c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955329"
---
# <a name="add-teacher"></a><span data-ttu-id="26a15-103">Добавление преподавателя</span><span class="sxs-lookup"><span data-stu-id="26a15-103">Add teacher</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26a15-104">Добавление преподавателя в класс.</span><span class="sxs-lookup"><span data-stu-id="26a15-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="26a15-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="26a15-105">Permissions</span></span>
<span data-ttu-id="26a15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26a15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26a15-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="26a15-108">Permission type</span></span>      | <span data-ttu-id="26a15-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="26a15-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="26a15-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="26a15-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="26a15-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a15-111">Not supported.</span></span>  |
|<span data-ttu-id="26a15-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="26a15-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="26a15-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="26a15-113">Not supported.</span></span>  |
|<span data-ttu-id="26a15-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="26a15-114">Application</span></span> | <span data-ttu-id="26a15-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26a15-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="26a15-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="26a15-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="26a15-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="26a15-117">Request headers</span></span>
| <span data-ttu-id="26a15-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="26a15-118">Header</span></span>       | <span data-ttu-id="26a15-119">Значение</span><span class="sxs-lookup"><span data-stu-id="26a15-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="26a15-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="26a15-120">Authorization</span></span>  | <span data-ttu-id="26a15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="26a15-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="26a15-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="26a15-123">Content-Type</span></span>  | <span data-ttu-id="26a15-124">application/json</span><span class="sxs-lookup"><span data-stu-id="26a15-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="26a15-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="26a15-125">Request body</span></span>
<span data-ttu-id="26a15-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="26a15-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="26a15-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="26a15-127">Response</span></span>
<span data-ttu-id="26a15-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="26a15-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26a15-129">Пример</span><span class="sxs-lookup"><span data-stu-id="26a15-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="26a15-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="26a15-130">Request</span></span>
<span data-ttu-id="26a15-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="26a15-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="26a15-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="26a15-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11017/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14011"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="26a15-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="26a15-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="26a15-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="26a15-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="26a15-135">C#</span><span class="sxs-lookup"><span data-stu-id="26a15-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationclass-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="26a15-136">Java</span><span class="sxs-lookup"><span data-stu-id="26a15-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationclass-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="26a15-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="26a15-137">Response</span></span>
<span data-ttu-id="26a15-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="26a15-138">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="26a15-p103">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="26a15-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
