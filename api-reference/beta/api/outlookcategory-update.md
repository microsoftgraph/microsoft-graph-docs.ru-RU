---
title: Обновление категории Outlook
description: 'Обновление перезаписываемого свойства **color** указанного объекта outlookCategory. Невозможно изменить свойство **DisplayName** '
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5030331f2dd38929a94d0f12e05e08d30b3a6bb5
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36414177"
---
# <a name="update-outlook-category"></a><span data-ttu-id="fd1bb-104">Обновление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="fd1bb-104">Update Outlook category</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd1bb-105">Обновление перезаписываемого свойства **color** указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="fd1bb-105">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="fd1bb-106">Нельзя изменить свойство **displayName** после создания категории.</span><span class="sxs-lookup"><span data-stu-id="fd1bb-106">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd1bb-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fd1bb-107">Permissions</span></span>
<span data-ttu-id="fd1bb-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fd1bb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd1bb-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fd1bb-110">Permission type</span></span>      | <span data-ttu-id="fd1bb-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fd1bb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd1bb-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fd1bb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd1bb-113">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd1bb-113">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="fd1bb-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fd1bb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd1bb-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd1bb-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="fd1bb-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fd1bb-116">Application</span></span> | <span data-ttu-id="fd1bb-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="fd1bb-117">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd1bb-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fd1bb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fd1bb-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fd1bb-119">Request headers</span></span>
| <span data-ttu-id="fd1bb-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fd1bb-120">Name</span></span>      |<span data-ttu-id="fd1bb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fd1bb-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fd1bb-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fd1bb-122">Authorization</span></span>  | <span data-ttu-id="fd1bb-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fd1bb-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd1bb-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fd1bb-125">Request body</span></span>
<span data-ttu-id="fd1bb-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="fd1bb-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="fd1bb-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd1bb-129">Property</span></span>     | <span data-ttu-id="fd1bb-130">Тип</span><span class="sxs-lookup"><span data-stu-id="fd1bb-130">Type</span></span>   |<span data-ttu-id="fd1bb-131">Описание</span><span class="sxs-lookup"><span data-stu-id="fd1bb-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fd1bb-132">color</span><span class="sxs-lookup"><span data-stu-id="fd1bb-132">color</span></span>|<span data-ttu-id="fd1bb-133">String</span><span class="sxs-lookup"><span data-stu-id="fd1bb-133">String</span></span>|<span data-ttu-id="fd1bb-134">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="fd1bb-134">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="fd1bb-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fd1bb-135">Response</span></span>

<span data-ttu-id="fd1bb-136">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="fd1bb-136">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fd1bb-137">Пример</span><span class="sxs-lookup"><span data-stu-id="fd1bb-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd1bb-138">Запрос</span><span class="sxs-lookup"><span data-stu-id="fd1bb-138">Request</span></span>
<span data-ttu-id="fd1bb-139">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fd1bb-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fd1bb-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd1bb-140">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="fd1bb-141">C#</span><span class="sxs-lookup"><span data-stu-id="fd1bb-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fd1bb-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd1bb-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fd1bb-143">Цель — C</span><span class="sxs-lookup"><span data-stu-id="fd1bb-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fd1bb-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="fd1bb-144">Response</span></span>
<span data-ttu-id="fd1bb-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fd1bb-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  ]
}
-->
