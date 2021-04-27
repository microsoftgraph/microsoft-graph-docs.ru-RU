---
title: Обновление категории Outlook
description: 'Обновление перезаписываемого свойства **color** указанного объекта outlookCategory. Невозможно изменить **свойство displayName** '
localization_priority: Normal
author: abheek-das
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: f570c805f93ad7be8b05dd2dc6ccdefe654128fd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055500"
---
# <a name="update-outlook-category"></a><span data-ttu-id="5a998-104">Обновление категории Outlook</span><span class="sxs-lookup"><span data-stu-id="5a998-104">Update Outlook category</span></span>

<span data-ttu-id="5a998-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a998-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a998-106">Обновление перезаписываемого свойства **color** указанного объекта [outlookCategory](../resources/outlookcategory.md).</span><span class="sxs-lookup"><span data-stu-id="5a998-106">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="5a998-107">Нельзя изменить свойство **displayName** после создания категории.</span><span class="sxs-lookup"><span data-stu-id="5a998-107">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a998-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5a998-108">Permissions</span></span>
<span data-ttu-id="5a998-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5a998-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5a998-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5a998-111">Permission type</span></span>      | <span data-ttu-id="5a998-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5a998-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5a998-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5a998-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5a998-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a998-114">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="5a998-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5a998-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a998-116">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a998-116">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="5a998-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="5a998-117">Application</span></span> | <span data-ttu-id="5a998-118">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="5a998-118">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a998-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5a998-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5a998-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5a998-120">Request headers</span></span>
| <span data-ttu-id="5a998-121">Имя</span><span class="sxs-lookup"><span data-stu-id="5a998-121">Name</span></span>      |<span data-ttu-id="5a998-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5a998-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5a998-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5a998-123">Authorization</span></span>  | <span data-ttu-id="5a998-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="5a998-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a998-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5a998-126">Request body</span></span>
<span data-ttu-id="5a998-p105">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="5a998-p105">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5a998-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="5a998-130">Property</span></span>     | <span data-ttu-id="5a998-131">Тип</span><span class="sxs-lookup"><span data-stu-id="5a998-131">Type</span></span>   |<span data-ttu-id="5a998-132">Описание</span><span class="sxs-lookup"><span data-stu-id="5a998-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a998-133">color</span><span class="sxs-lookup"><span data-stu-id="5a998-133">color</span></span>|<span data-ttu-id="5a998-134">String</span><span class="sxs-lookup"><span data-stu-id="5a998-134">String</span></span>|<span data-ttu-id="5a998-135">Предустановленная константа, которая характеризует категорию и сопоставлена с одним из 25 предопределенных цветов.</span><span class="sxs-lookup"><span data-stu-id="5a998-135">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="5a998-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="5a998-136">Response</span></span>

<span data-ttu-id="5a998-137">В случае успешного выполнения этот метод возвращает код ответа `200 OK` и объект [outlookCategory](../resources/outlookcategory.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="5a998-137">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5a998-138">Пример</span><span class="sxs-lookup"><span data-stu-id="5a998-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5a998-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="5a998-139">Request</span></span>
<span data-ttu-id="5a998-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="5a998-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5a998-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a998-141">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5a998-142">C#</span><span class="sxs-lookup"><span data-stu-id="5a998-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-outlookcategory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5a998-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a998-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-outlookcategory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a998-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a998-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-outlookcategory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5a998-145">Java</span><span class="sxs-lookup"><span data-stu-id="5a998-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-outlookcategory-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5a998-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="5a998-146">Response</span></span>
<span data-ttu-id="5a998-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="5a998-147">Here is an example of the response.</span></span> <span data-ttu-id="5a998-148">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5a998-148">Note: The response object shown here might be shortened for readability.</span></span>
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


