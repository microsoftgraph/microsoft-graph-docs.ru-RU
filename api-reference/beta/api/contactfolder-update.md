---
title: Обновление объекта contactFolder
description: Обновление свойств объекта contactFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: da438b455cc444ff3d79d1b7d9d5b8db94c83074
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417902"
---
# <a name="update-contactfolder"></a><span data-ttu-id="8c491-103">Обновление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="8c491-103">Update contactfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c491-104">Обновление свойств объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="8c491-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="8c491-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="8c491-105">Permissions</span></span>
<span data-ttu-id="8c491-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c491-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="8c491-108">Permission type</span></span>      | <span data-ttu-id="8c491-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="8c491-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8c491-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="8c491-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8c491-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c491-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8c491-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="8c491-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c491-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c491-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="8c491-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="8c491-114">Application</span></span> | <span data-ttu-id="8c491-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8c491-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c491-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="8c491-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="8c491-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="8c491-117">Request headers</span></span>
| <span data-ttu-id="8c491-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="8c491-118">Header</span></span>       | <span data-ttu-id="8c491-119">Значение</span><span class="sxs-lookup"><span data-stu-id="8c491-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8c491-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="8c491-120">Authorization</span></span>  | <span data-ttu-id="8c491-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c491-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8c491-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8c491-123">Content-Type</span></span>  | <span data-ttu-id="8c491-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="8c491-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8c491-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="8c491-126">Request body</span></span>
<span data-ttu-id="8c491-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="8c491-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="8c491-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c491-130">Property</span></span>     | <span data-ttu-id="8c491-131">Тип</span><span class="sxs-lookup"><span data-stu-id="8c491-131">Type</span></span>   |<span data-ttu-id="8c491-132">Описание</span><span class="sxs-lookup"><span data-stu-id="8c491-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c491-133">displayName</span><span class="sxs-lookup"><span data-stu-id="8c491-133">displayName</span></span>|<span data-ttu-id="8c491-134">String</span><span class="sxs-lookup"><span data-stu-id="8c491-134">String</span></span>|<span data-ttu-id="8c491-135">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="8c491-135">The folder's display name.</span></span>|
|<span data-ttu-id="8c491-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="8c491-136">parentFolderId</span></span>|<span data-ttu-id="8c491-137">String</span><span class="sxs-lookup"><span data-stu-id="8c491-137">String</span></span>|<span data-ttu-id="8c491-138">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="8c491-138">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="8c491-139">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="8c491-139">wellKnownName</span></span>|<span data-ttu-id="8c491-140">string</span><span class="sxs-lookup"><span data-stu-id="8c491-140">string</span></span>|<span data-ttu-id="8c491-141">Имя папки, если она является распознаваемой папкой.</span><span class="sxs-lookup"><span data-stu-id="8c491-141">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="8c491-142">В `contacts` настоящее время это единственная распознанная папка контактов.</span><span class="sxs-lookup"><span data-stu-id="8c491-142">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="8c491-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c491-143">Response</span></span>

<span data-ttu-id="8c491-144">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="8c491-144">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8c491-145">Пример</span><span class="sxs-lookup"><span data-stu-id="8c491-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8c491-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="8c491-146">Request</span></span>
<span data-ttu-id="8c491-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="8c491-147">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="8c491-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c491-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_contactfolder"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/contactFolders/{id}
Content-type: application/json
Content-length: 84

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8c491-149">C#</span><span class="sxs-lookup"><span data-stu-id="8c491-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8c491-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c491-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8c491-151">Цель — C</span><span class="sxs-lookup"><span data-stu-id="8c491-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8c491-152">Отклик</span><span class="sxs-lookup"><span data-stu-id="8c491-152">Response</span></span>
<span data-ttu-id="8c491-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="8c491-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contactFolder"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 104

{
  "parentFolderId": "parentFolderId-value",
  "displayName": "displayName-value",
  "wellKnownName": "wellKnownName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update contactfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
