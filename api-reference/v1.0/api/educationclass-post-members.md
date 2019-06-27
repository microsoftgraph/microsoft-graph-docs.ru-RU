---
title: Добавление учащегося
description: Добавление участника курса.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ac2cca18a733ac99bc8aadb9d0bbaae9a6e69455
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275154"
---
# <a name="add-a-student"></a><span data-ttu-id="7f1b8-103">Добавление учащегося</span><span class="sxs-lookup"><span data-stu-id="7f1b8-103">Add a student</span></span>

<span data-ttu-id="7f1b8-104">Добавление участника курса.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f1b8-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="7f1b8-105">Permissions</span></span>
<span data-ttu-id="7f1b8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7f1b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f1b8-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="7f1b8-108">Permission type</span></span>      | <span data-ttu-id="7f1b8-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="7f1b8-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7f1b8-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="7f1b8-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="7f1b8-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-111">Not supported.</span></span>  |
|<span data-ttu-id="7f1b8-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="7f1b8-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="7f1b8-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-113">Not supported.</span></span>  |
|<span data-ttu-id="7f1b8-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="7f1b8-114">Application</span></span> | <span data-ttu-id="7f1b8-115">EduRoster. ReadWrite. ALL, Plus Member. Read. Hidden</span><span class="sxs-lookup"><span data-stu-id="7f1b8-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="7f1b8-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="7f1b8-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="7f1b8-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="7f1b8-117">Request headers</span></span>
| <span data-ttu-id="7f1b8-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="7f1b8-118">Header</span></span>       | <span data-ttu-id="7f1b8-119">Значение</span><span class="sxs-lookup"><span data-stu-id="7f1b8-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="7f1b8-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="7f1b8-120">Authorization</span></span>  | <span data-ttu-id="7f1b8-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7f1b8-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f1b8-123">Content-Type</span></span>  | <span data-ttu-id="7f1b8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7f1b8-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="7f1b8-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="7f1b8-125">Request body</span></span>
<span data-ttu-id="7f1b8-126">В теле запроса предоставьте описание объекта [educationUser](../resources/educationuser.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="7f1b8-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f1b8-127">Response</span></span>
<span data-ttu-id="7f1b8-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f1b8-129">Пример</span><span class="sxs-lookup"><span data-stu-id="7f1b8-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7f1b8-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="7f1b8-130">Request</span></span>
<span data-ttu-id="7f1b8-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-131">The following is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="7f1b8-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="7f1b8-132">Response</span></span>
<span data-ttu-id="7f1b8-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="7f1b8-133">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="7f1b8-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="7f1b8-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7f1b8-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="7f1b8-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationclass-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="7f1b8-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="7f1b8-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationclass-Objective-C-snippets.md)]
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
    "Error: /api-reference/v1.0/api/educationclass-post-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/educationclass-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
