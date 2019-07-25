---
title: Добавление educationUser в educationSchool
description: Добавление пользователя в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 975de4625c7b60276521866b26a2753049c7e45f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35860339"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="c83ed-103">Добавление educationUser в educationSchool</span><span class="sxs-lookup"><span data-stu-id="c83ed-103">Add educationUser to an educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c83ed-104">Добавление пользователя в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="c83ed-104">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="c83ed-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c83ed-105">Permissions</span></span>

<span data-ttu-id="c83ed-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c83ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c83ed-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c83ed-108">Permission type</span></span>                        | <span data-ttu-id="c83ed-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c83ed-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="c83ed-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c83ed-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c83ed-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c83ed-111">Not supported.</span></span>                              |
| <span data-ttu-id="c83ed-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c83ed-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c83ed-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c83ed-113">Not supported.</span></span>                              |
| <span data-ttu-id="c83ed-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c83ed-114">Application</span></span>                            | <span data-ttu-id="c83ed-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c83ed-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="c83ed-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c83ed-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```

## <a name="request-headers"></a><span data-ttu-id="c83ed-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c83ed-117">Request headers</span></span>

| <span data-ttu-id="c83ed-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c83ed-118">Header</span></span>        | <span data-ttu-id="c83ed-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c83ed-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="c83ed-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c83ed-120">Authorization</span></span> | <span data-ttu-id="c83ed-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c83ed-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c83ed-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c83ed-123">Content-Type</span></span>  | <span data-ttu-id="c83ed-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c83ed-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="c83ed-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c83ed-125">Request body</span></span>

<span data-ttu-id="c83ed-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c83ed-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c83ed-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c83ed-127">Response</span></span>

<span data-ttu-id="c83ed-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c83ed-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c83ed-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c83ed-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c83ed-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c83ed-130">Request</span></span>

<span data-ttu-id="c83ed-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c83ed-131">The following is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c83ed-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c83ed-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->

```http
POST https://graph.microsoft.com/beta/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14008"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c83ed-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c83ed-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c83ed-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c83ed-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="ctabcsharp"></a>[<span data-ttu-id="c83ed-135">C#</span><span class="sxs-lookup"><span data-stu-id="c83ed-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c83ed-136">Java</span><span class="sxs-lookup"><span data-stu-id="c83ed-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationuser-from-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c83ed-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="c83ed-137">Response</span></span>

<span data-ttu-id="c83ed-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c83ed-138">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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
