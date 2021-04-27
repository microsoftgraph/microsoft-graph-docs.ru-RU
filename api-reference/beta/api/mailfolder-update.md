---
title: Обновление mailFolder
description: Обновление свойств объекта mailFolder.
author: abheek-das
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: b6039bf189d88c46612fab8ec71ac6ae4eb7909b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053008"
---
# <a name="update-mailfolder"></a><span data-ttu-id="87cb1-103">Обновление mailFolder</span><span class="sxs-lookup"><span data-stu-id="87cb1-103">Update mailFolder</span></span>

<span data-ttu-id="87cb1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87cb1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="87cb1-105">Обновление свойств [объекта mailFolder.](../resources/mailfolder.md)</span><span class="sxs-lookup"><span data-stu-id="87cb1-105">Update the properties of [mailFolder](../resources/mailfolder.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="87cb1-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="87cb1-106">Permissions</span></span>
<span data-ttu-id="87cb1-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87cb1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87cb1-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="87cb1-109">Permission type</span></span>      | <span data-ttu-id="87cb1-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="87cb1-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="87cb1-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="87cb1-111">Delegated (work or school account)</span></span> | <span data-ttu-id="87cb1-112">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87cb1-112">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="87cb1-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="87cb1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="87cb1-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87cb1-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="87cb1-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="87cb1-115">Application</span></span> | <span data-ttu-id="87cb1-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="87cb1-116">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="87cb1-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="87cb1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="87cb1-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="87cb1-118">Request headers</span></span>
| <span data-ttu-id="87cb1-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="87cb1-119">Header</span></span>       | <span data-ttu-id="87cb1-120">Значение</span><span class="sxs-lookup"><span data-stu-id="87cb1-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="87cb1-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="87cb1-121">Authorization</span></span>  | <span data-ttu-id="87cb1-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87cb1-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="87cb1-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="87cb1-124">Content-Type</span></span>  | <span data-ttu-id="87cb1-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="87cb1-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="87cb1-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="87cb1-127">Request body</span></span>
<span data-ttu-id="87cb1-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="87cb1-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="87cb1-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="87cb1-131">Property</span></span>     | <span data-ttu-id="87cb1-132">Тип</span><span class="sxs-lookup"><span data-stu-id="87cb1-132">Type</span></span>   |<span data-ttu-id="87cb1-133">Описание</span><span class="sxs-lookup"><span data-stu-id="87cb1-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="87cb1-134">displayName</span><span class="sxs-lookup"><span data-stu-id="87cb1-134">displayName</span></span>|<span data-ttu-id="87cb1-135">Строка</span><span class="sxs-lookup"><span data-stu-id="87cb1-135">String</span></span>|<span data-ttu-id="87cb1-136">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="87cb1-136">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="87cb1-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="87cb1-137">Response</span></span>
<span data-ttu-id="87cb1-138">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="87cb1-138">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87cb1-139">Пример</span><span class="sxs-lookup"><span data-stu-id="87cb1-139">Example</span></span>
#### <a name="request"></a><span data-ttu-id="87cb1-140">Запрос</span><span class="sxs-lookup"><span data-stu-id="87cb1-140">Request</span></span>
<span data-ttu-id="87cb1-141">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="87cb1-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="87cb1-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="87cb1-142">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="87cb1-143">C#</span><span class="sxs-lookup"><span data-stu-id="87cb1-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="87cb1-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="87cb1-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="87cb1-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="87cb1-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="87cb1-146">Java</span><span class="sxs-lookup"><span data-stu-id="87cb1-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-mailfolder-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="87cb1-147">Отклик</span><span class="sxs-lookup"><span data-stu-id="87cb1-147">Response</span></span>
<span data-ttu-id="87cb1-148">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="87cb1-148">The following is an example of the response.</span></span>
><span data-ttu-id="87cb1-149">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="87cb1-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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


