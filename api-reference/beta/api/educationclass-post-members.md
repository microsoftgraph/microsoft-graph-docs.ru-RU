---
title: Добавление учащегося
description: Добавление участника курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: dc3702b96137e7e8631662d69ecc98e1bf7c9ddf
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/02/2019
ms.locfileid: "35435992"
---
# <a name="add-a-student"></a><span data-ttu-id="c28c3-103">Добавление учащегося</span><span class="sxs-lookup"><span data-stu-id="c28c3-103">Add a student</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c28c3-104">Добавление участника курса.</span><span class="sxs-lookup"><span data-stu-id="c28c3-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="c28c3-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c28c3-105">Permissions</span></span>
<span data-ttu-id="c28c3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c28c3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c28c3-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c28c3-108">Permission type</span></span>      | <span data-ttu-id="c28c3-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c28c3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c28c3-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c28c3-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c28c3-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c28c3-111">Not supported.</span></span>  |
|<span data-ttu-id="c28c3-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c28c3-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c28c3-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c28c3-113">Not supported.</span></span>  |
|<span data-ttu-id="c28c3-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c28c3-114">Application</span></span> | <span data-ttu-id="c28c3-115">EduRoster. ReadWrite. ALL, Plus Member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="c28c3-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c28c3-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c28c3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="c28c3-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c28c3-117">Request headers</span></span>
| <span data-ttu-id="c28c3-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="c28c3-118">Header</span></span>       | <span data-ttu-id="c28c3-119">Значение</span><span class="sxs-lookup"><span data-stu-id="c28c3-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c28c3-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c28c3-120">Authorization</span></span>  | <span data-ttu-id="c28c3-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c28c3-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c28c3-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c28c3-123">Content-Type</span></span>  | <span data-ttu-id="c28c3-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c28c3-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c28c3-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c28c3-125">Request body</span></span>
<span data-ttu-id="c28c3-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c28c3-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="c28c3-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="c28c3-127">Response</span></span>
<span data-ttu-id="c28c3-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="c28c3-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c28c3-129">Пример</span><span class="sxs-lookup"><span data-stu-id="c28c3-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c28c3-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="c28c3-130">Request</span></span>
<span data-ttu-id="c28c3-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c28c3-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c28c3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="c28c3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/13015"
}
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c28c3-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="c28c3-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationuser-from-educationclass-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c28c3-134">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c28c3-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationuser-from-educationclass-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c28c3-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="c28c3-135">Response</span></span>
<span data-ttu-id="c28c3-136">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="c28c3-136">The following is an example of the response.</span></span> 


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
