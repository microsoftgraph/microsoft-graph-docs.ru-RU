---
title: Добавление educationUser в educationSchool
description: Добавление пользователя в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2fef72e17d512a0637a7bbc10c0a41ebbcd351e0
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587801"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="9b15c-103">Добавление educationUser в educationSchool</span><span class="sxs-lookup"><span data-stu-id="9b15c-103">Add educationUser to an educationSchool</span></span>

<span data-ttu-id="9b15c-104">Добавление пользователя в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="9b15c-104">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b15c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9b15c-105">Permissions</span></span>
<span data-ttu-id="9b15c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9b15c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9b15c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9b15c-108">Permission type</span></span>      | <span data-ttu-id="9b15c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9b15c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9b15c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9b15c-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9b15c-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b15c-111">Not supported.</span></span>  |
|<span data-ttu-id="9b15c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9b15c-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9b15c-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9b15c-113">Not supported.</span></span>  |
|<span data-ttu-id="9b15c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9b15c-114">Application</span></span> | <span data-ttu-id="9b15c-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9b15c-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9b15c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9b15c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9b15c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9b15c-117">Request headers</span></span>
| <span data-ttu-id="9b15c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="9b15c-118">Header</span></span>       | <span data-ttu-id="9b15c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="9b15c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9b15c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9b15c-120">Authorization</span></span>  | <span data-ttu-id="9b15c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9b15c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9b15c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9b15c-123">Content-Type</span></span>  | <span data-ttu-id="9b15c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9b15c-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9b15c-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9b15c-125">Request body</span></span>
<span data-ttu-id="9b15c-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b15c-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9b15c-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b15c-127">Response</span></span>
<span data-ttu-id="9b15c-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="9b15c-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b15c-129">Пример</span><span class="sxs-lookup"><span data-stu-id="9b15c-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9b15c-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="9b15c-130">Request</span></span>
<span data-ttu-id="9b15c-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9b15c-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{id}/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="9b15c-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="9b15c-132">Response</span></span>
<span data-ttu-id="9b15c-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9b15c-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9b15c-134">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="9b15c-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9b15c-135">Язык</span><span class="sxs-lookup"><span data-stu-id="9b15c-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationschool-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/educationschool-post-users.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
