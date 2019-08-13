---
title: Обновление mailFolder
description: Обновление свойств объекта mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 6517386c4c21df35ae8df843de5734142a249f68
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347089"
---
# <a name="update-mailfolder"></a><span data-ttu-id="da24c-103">Обновление mailFolder</span><span class="sxs-lookup"><span data-stu-id="da24c-103">Update mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da24c-104">Обновление свойств объекта [mailFolder](../resources/mailfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="da24c-104">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="da24c-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="da24c-105">Permissions</span></span>
<span data-ttu-id="da24c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="da24c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da24c-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="da24c-108">Permission type</span></span>      | <span data-ttu-id="da24c-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="da24c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da24c-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="da24c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="da24c-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da24c-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="da24c-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="da24c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="da24c-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da24c-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="da24c-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="da24c-114">Application</span></span> | <span data-ttu-id="da24c-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="da24c-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="da24c-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="da24c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="da24c-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="da24c-117">Request headers</span></span>
| <span data-ttu-id="da24c-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="da24c-118">Header</span></span>       | <span data-ttu-id="da24c-119">Значение</span><span class="sxs-lookup"><span data-stu-id="da24c-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da24c-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="da24c-120">Authorization</span></span>  | <span data-ttu-id="da24c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da24c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da24c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da24c-123">Content-Type</span></span>  | <span data-ttu-id="da24c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="da24c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da24c-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="da24c-126">Request body</span></span>
<span data-ttu-id="da24c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="da24c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="da24c-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="da24c-130">Property</span></span>     | <span data-ttu-id="da24c-131">Тип</span><span class="sxs-lookup"><span data-stu-id="da24c-131">Type</span></span>   |<span data-ttu-id="da24c-132">Описание</span><span class="sxs-lookup"><span data-stu-id="da24c-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="da24c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="da24c-133">displayName</span></span>|<span data-ttu-id="da24c-134">Строка</span><span class="sxs-lookup"><span data-stu-id="da24c-134">String</span></span>|<span data-ttu-id="da24c-135">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="da24c-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="da24c-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="da24c-136">Response</span></span>
<span data-ttu-id="da24c-137">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="da24c-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da24c-138">Пример</span><span class="sxs-lookup"><span data-stu-id="da24c-138">Example</span></span>
#### <a name="request"></a><span data-ttu-id="da24c-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="da24c-139">Request</span></span>
<span data-ttu-id="da24c-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="da24c-140">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="da24c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="da24c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="da24c-142">C#</span><span class="sxs-lookup"><span data-stu-id="da24c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="da24c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="da24c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="da24c-144">Цель — C</span><span class="sxs-lookup"><span data-stu-id="da24c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="da24c-145">Java</span><span class="sxs-lookup"><span data-stu-id="da24c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="da24c-146">Отклик</span><span class="sxs-lookup"><span data-stu-id="da24c-146">Response</span></span>
<span data-ttu-id="da24c-147">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="da24c-147">The following is an example of the response.</span></span>
><span data-ttu-id="da24c-148">**Примечание.**  Объект ответа, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="da24c-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="da24c-149">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="da24c-149">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.mailFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 179

{
    "id": "AAMkAGVmMDEzM",
    "displayName": "displayName-value",
    "parentFolderId": "AAMkAGVmMDEzI",
    "childFolderCount": 2,
    "unreadItemCount": 59,
    "totalItemCount": 60,
    "wellKnownName": "inbox"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
