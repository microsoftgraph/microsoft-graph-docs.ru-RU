---
title: Обновление объекта contactFolder
description: Обновление свойств объекта contactFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 4380fafe842af304b8dfd99b86cae3d499669b03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42436806"
---
# <a name="update-contactfolder"></a><span data-ttu-id="a7c8c-103">Обновление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="a7c8c-103">Update contactfolder</span></span>

<span data-ttu-id="a7c8c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a7c8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7c8c-105">Обновление свойств объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-105">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="a7c8c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a7c8c-106">Permissions</span></span>
<span data-ttu-id="a7c8c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7c8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c8c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a7c8c-109">Permission type</span></span>      | <span data-ttu-id="a7c8c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a7c8c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7c8c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a7c8c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a7c8c-112">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7c8c-112">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a7c8c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a7c8c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7c8c-114">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7c8c-114">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="a7c8c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a7c8c-115">Application</span></span> | <span data-ttu-id="a7c8c-116">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7c8c-116">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7c8c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a7c8c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a7c8c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a7c8c-118">Request headers</span></span>
| <span data-ttu-id="a7c8c-119">Заголовок</span><span class="sxs-lookup"><span data-stu-id="a7c8c-119">Header</span></span>       | <span data-ttu-id="a7c8c-120">Значение</span><span class="sxs-lookup"><span data-stu-id="a7c8c-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7c8c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a7c8c-121">Authorization</span></span>  | <span data-ttu-id="a7c8c-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a7c8c-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a7c8c-124">Content-Type</span></span>  | <span data-ttu-id="a7c8c-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7c8c-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a7c8c-127">Request body</span></span>
<span data-ttu-id="a7c8c-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a7c8c-131">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7c8c-131">Property</span></span>     | <span data-ttu-id="a7c8c-132">Тип</span><span class="sxs-lookup"><span data-stu-id="a7c8c-132">Type</span></span>   |<span data-ttu-id="a7c8c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a7c8c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a7c8c-134">displayName</span><span class="sxs-lookup"><span data-stu-id="a7c8c-134">displayName</span></span>|<span data-ttu-id="a7c8c-135">String</span><span class="sxs-lookup"><span data-stu-id="a7c8c-135">String</span></span>|<span data-ttu-id="a7c8c-136">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-136">The folder's display name.</span></span>|
|<span data-ttu-id="a7c8c-137">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="a7c8c-137">parentFolderId</span></span>|<span data-ttu-id="a7c8c-138">String</span><span class="sxs-lookup"><span data-stu-id="a7c8c-138">String</span></span>|<span data-ttu-id="a7c8c-139">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-139">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="a7c8c-140">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="a7c8c-140">wellKnownName</span></span>|<span data-ttu-id="a7c8c-141">строка</span><span class="sxs-lookup"><span data-stu-id="a7c8c-141">string</span></span>|<span data-ttu-id="a7c8c-142">Имя папки, если она является распознаваемой папкой.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-142">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="a7c8c-143">В `contacts` настоящее время это единственная распознанная папка контактов.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-143">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="a7c8c-144">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7c8c-144">Response</span></span>

<span data-ttu-id="a7c8c-145">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-145">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7c8c-146">Пример</span><span class="sxs-lookup"><span data-stu-id="a7c8c-146">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7c8c-147">Запрос</span><span class="sxs-lookup"><span data-stu-id="a7c8c-147">Request</span></span>
<span data-ttu-id="a7c8c-148">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-148">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7c8c-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7c8c-149">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a7c8c-150">C#</span><span class="sxs-lookup"><span data-stu-id="a7c8c-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-contactfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7c8c-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7c8c-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-contactfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7c8c-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7c8c-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-contactfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7c8c-153">Отклик</span><span class="sxs-lookup"><span data-stu-id="a7c8c-153">Response</span></span>
<span data-ttu-id="a7c8c-p106">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="a7c8c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
