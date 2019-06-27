---
title: Обновление категории Outlook
description: 'Обновление перезаписываемого свойства **color** указанного объекта outlookCategory. Невозможно изменить свойство **DisplayName** '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7ea8beeb60141089662e46eb737c8dd3a2ac74c9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266817"
---
# <a name="update-outlook-category"></a><span data-ttu-id="682f2-104">Обновление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="682f2-104">Update Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="682f2-105">Обновление перезаписываемого свойства **color** указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="682f2-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="682f2-106">Нельзя изменить свойство **displayName** после создания категории.</span><span class="sxs-lookup"><span data-stu-id="682f2-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="682f2-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="682f2-107">Permissions</span></span>
<span data-ttu-id="682f2-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="682f2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="682f2-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="682f2-110">Permission type</span></span>      | <span data-ttu-id="682f2-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="682f2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="682f2-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="682f2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="682f2-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="682f2-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="682f2-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="682f2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="682f2-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="682f2-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="682f2-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="682f2-116">Application</span></span> | <span data-ttu-id="682f2-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="682f2-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="682f2-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="682f2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="682f2-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="682f2-119">Request headers</span></span>
| <span data-ttu-id="682f2-120">Имя</span><span class="sxs-lookup"><span data-stu-id="682f2-120">Name</span></span>      |<span data-ttu-id="682f2-121">Описание</span><span class="sxs-lookup"><span data-stu-id="682f2-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="682f2-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="682f2-122">Authorization</span></span>  | <span data-ttu-id="682f2-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="682f2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="682f2-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="682f2-125">Request body</span></span>
<span data-ttu-id="682f2-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="682f2-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="682f2-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="682f2-129">Property</span></span>     | <span data-ttu-id="682f2-130">Тип</span><span class="sxs-lookup"><span data-stu-id="682f2-130">Type</span></span>   |<span data-ttu-id="682f2-131">Описание</span><span class="sxs-lookup"><span data-stu-id="682f2-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="682f2-132">color</span><span class="sxs-lookup"><span data-stu-id="682f2-132">color</span></span>|<span data-ttu-id="682f2-133">String</span><span class="sxs-lookup"><span data-stu-id="682f2-133">String</span></span>|<span data-ttu-id="682f2-134">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="682f2-134">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="682f2-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="682f2-135">Response</span></span>

<span data-ttu-id="682f2-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="682f2-136">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="682f2-137">Пример</span><span class="sxs-lookup"><span data-stu-id="682f2-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="682f2-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="682f2-138">Request</span></span>
<span data-ttu-id="682f2-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="682f2-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/masterCategories/bac262b7-485d-4739-b436-e31467d64fac
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="682f2-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="682f2-140">Response</span></span>
<span data-ttu-id="682f2-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="682f2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="682f2-144">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="682f2-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="682f2-145">C#</span><span class="sxs-lookup"><span data-stu-id="682f2-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_outlookcategory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="682f2-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="682f2-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_outlookcategory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="682f2-147">Цель — C</span><span class="sxs-lookup"><span data-stu-id="682f2-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_outlookcategory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/outlookcategory-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/outlookcategory-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/outlookcategory-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
