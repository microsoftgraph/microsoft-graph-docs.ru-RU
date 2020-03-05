---
title: Добавление educationUser в educationSchool
description: Добавление пользователя в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 6f9e46d7edad0b73126f2c4dcc1747e828b79b6e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42425235"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="dda15-103">Добавление educationUser в educationSchool</span><span class="sxs-lookup"><span data-stu-id="dda15-103">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="dda15-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="dda15-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dda15-105">Добавление пользователя в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="dda15-105">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="dda15-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dda15-106">Permissions</span></span>

<span data-ttu-id="dda15-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dda15-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dda15-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dda15-109">Permission type</span></span>                        | <span data-ttu-id="dda15-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dda15-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="dda15-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dda15-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="dda15-112">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dda15-112">Not supported.</span></span>                              |
| <span data-ttu-id="dda15-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dda15-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dda15-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dda15-114">Not supported.</span></span>                              |
| <span data-ttu-id="dda15-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dda15-115">Application</span></span>                            | <span data-ttu-id="dda15-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dda15-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="dda15-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dda15-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```

## <a name="request-headers"></a><span data-ttu-id="dda15-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dda15-118">Request headers</span></span>

| <span data-ttu-id="dda15-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="dda15-119">Header</span></span>        | <span data-ttu-id="dda15-120">Значение</span><span class="sxs-lookup"><span data-stu-id="dda15-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="dda15-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="dda15-121">Authorization</span></span> | <span data-ttu-id="dda15-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="dda15-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dda15-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dda15-124">Content-Type</span></span>  | <span data-ttu-id="dda15-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dda15-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="dda15-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dda15-126">Request body</span></span>

<span data-ttu-id="dda15-127">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="dda15-127">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="dda15-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dda15-128">Response</span></span>

<span data-ttu-id="dda15-129">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="dda15-129">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dda15-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dda15-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dda15-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dda15-131">Request</span></span>

<span data-ttu-id="dda15-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dda15-132">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="dda15-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dda15-133">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="dda15-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dda15-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dda15-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dda15-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="dda15-136">C#</span><span class="sxs-lookup"><span data-stu-id="dda15-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationuser-from-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dda15-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="dda15-137">Response</span></span>

<span data-ttu-id="dda15-138">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dda15-138">The following is an example of the response.</span></span> 

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
