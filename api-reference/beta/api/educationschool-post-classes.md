---
title: Добавление educationClass к educationSchool
description: Добавление класса в учебное заведение.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2f58e67dfbd96875b4e3006741211969953d5b03
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259572"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="fa1eb-103">Добавление educationClass к educationSchool</span><span class="sxs-lookup"><span data-stu-id="fa1eb-103">Add educationClass to educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa1eb-104">Добавление класса в учебное заведение.</span><span class="sxs-lookup"><span data-stu-id="fa1eb-104">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa1eb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fa1eb-105">Permissions</span></span>
<span data-ttu-id="fa1eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa1eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa1eb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fa1eb-108">Permission type</span></span>      | <span data-ttu-id="fa1eb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fa1eb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa1eb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fa1eb-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="fa1eb-111">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa1eb-111">Not supported.</span></span>  |
|<span data-ttu-id="fa1eb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fa1eb-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="fa1eb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fa1eb-113">Not supported.</span></span>  |
|<span data-ttu-id="fa1eb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fa1eb-114">Application</span></span> | <span data-ttu-id="fa1eb-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa1eb-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="fa1eb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fa1eb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="fa1eb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fa1eb-117">Request headers</span></span>
| <span data-ttu-id="fa1eb-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="fa1eb-118">Header</span></span>       | <span data-ttu-id="fa1eb-119">Значение</span><span class="sxs-lookup"><span data-stu-id="fa1eb-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa1eb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fa1eb-120">Authorization</span></span>  | <span data-ttu-id="fa1eb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fa1eb-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fa1eb-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fa1eb-123">Content-Type</span></span>  | <span data-ttu-id="fa1eb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fa1eb-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fa1eb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fa1eb-125">Request body</span></span>
<span data-ttu-id="fa1eb-126">В теле запроса предоставьте описание объекта [educationClass](../resources/educationclass.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fa1eb-126">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="fa1eb-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa1eb-127">Response</span></span>
<span data-ttu-id="fa1eb-128">При успешном выполнении этот метод возвратит код отклика `204 No Content` и объект [educationClass](../resources/educationclass.md) в теле отклика.</span><span class="sxs-lookup"><span data-stu-id="fa1eb-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa1eb-129">Пример</span><span class="sxs-lookup"><span data-stu-id="fa1eb-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fa1eb-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="fa1eb-130">Request</span></span>
<span data-ttu-id="fa1eb-131">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fa1eb-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="fa1eb-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="fa1eb-132">Response</span></span> 
<span data-ttu-id="fa1eb-133">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fa1eb-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="fa1eb-134">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="fa1eb-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa1eb-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="fa1eb-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationclass_from_educationschool-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="fa1eb-136">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fa1eb-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_educationclass_from_educationschool-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationschool-post-classes.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationschool-post-classes.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
