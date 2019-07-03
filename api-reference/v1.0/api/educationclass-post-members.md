---
title: Добавление учащегося
description: Добавление участника курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 49e2ef6ba4401fb95672b67d693cf4a223f8137f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35449934"
---
# <a name="add-a-student"></a><span data-ttu-id="825c7-103">Добавление учащегося</span><span class="sxs-lookup"><span data-stu-id="825c7-103">Add a student</span></span>

<span data-ttu-id="825c7-104">Добавление участника курса.</span><span class="sxs-lookup"><span data-stu-id="825c7-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="825c7-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="825c7-105">Permissions</span></span>
<span data-ttu-id="825c7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="825c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="825c7-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="825c7-108">Permission type</span></span>      | <span data-ttu-id="825c7-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="825c7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="825c7-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="825c7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="825c7-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="825c7-111">Not supported.</span></span>  |
|<span data-ttu-id="825c7-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="825c7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="825c7-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="825c7-113">Not supported.</span></span>  |
|<span data-ttu-id="825c7-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="825c7-114">Application</span></span> | <span data-ttu-id="825c7-115">EduRoster. ReadWrite. ALL, Plus Member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="825c7-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="825c7-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="825c7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="825c7-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="825c7-117">Request headers</span></span>
| <span data-ttu-id="825c7-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="825c7-118">Header</span></span>       | <span data-ttu-id="825c7-119">Значение</span><span class="sxs-lookup"><span data-stu-id="825c7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="825c7-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="825c7-120">Authorization</span></span>  | <span data-ttu-id="825c7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="825c7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="825c7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="825c7-123">Content-Type</span></span>  | <span data-ttu-id="825c7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="825c7-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="825c7-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="825c7-125">Request body</span></span>
<span data-ttu-id="825c7-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="825c7-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="825c7-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="825c7-127">Response</span></span>
<span data-ttu-id="825c7-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="825c7-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="825c7-129">Пример</span><span class="sxs-lookup"><span data-stu-id="825c7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="825c7-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="825c7-130">Request</span></span>
<span data-ttu-id="825c7-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="825c7-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="825c7-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="825c7-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/13015"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="825c7-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="825c7-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="825c7-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="825c7-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="825c7-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="825c7-135">Response</span></span>
<span data-ttu-id="825c7-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="825c7-136">The following is an example of the response.</span></span> 


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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
