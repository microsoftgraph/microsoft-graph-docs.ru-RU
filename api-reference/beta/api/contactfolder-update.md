---
title: Обновление объекта contactFolder
description: Обновление свойств объекта contactFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a01cc70222205bcafd5cd892561b1ca831f51a59
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35261240"
---
# <a name="update-contactfolder"></a><span data-ttu-id="e4d91-103">Обновление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="e4d91-103">Update contactfolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4d91-104">Обновление свойств объекта contactFolder.</span><span class="sxs-lookup"><span data-stu-id="e4d91-104">Update the properties of contactfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="e4d91-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e4d91-105">Permissions</span></span>
<span data-ttu-id="e4d91-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e4d91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4d91-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e4d91-108">Permission type</span></span>      | <span data-ttu-id="e4d91-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e4d91-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e4d91-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e4d91-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e4d91-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d91-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e4d91-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e4d91-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e4d91-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d91-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="e4d91-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e4d91-114">Application</span></span> | <span data-ttu-id="e4d91-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e4d91-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="e4d91-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e4d91-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/contactFolders/{id}
PATCH /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="e4d91-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e4d91-117">Request headers</span></span>
| <span data-ttu-id="e4d91-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="e4d91-118">Header</span></span>       | <span data-ttu-id="e4d91-119">Значение</span><span class="sxs-lookup"><span data-stu-id="e4d91-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e4d91-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e4d91-120">Authorization</span></span>  | <span data-ttu-id="e4d91-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4d91-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e4d91-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e4d91-123">Content-Type</span></span>  | <span data-ttu-id="e4d91-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e4d91-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e4d91-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e4d91-126">Request body</span></span>
<span data-ttu-id="e4d91-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="e4d91-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e4d91-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4d91-130">Property</span></span>     | <span data-ttu-id="e4d91-131">Тип</span><span class="sxs-lookup"><span data-stu-id="e4d91-131">Type</span></span>   |<span data-ttu-id="e4d91-132">Описание</span><span class="sxs-lookup"><span data-stu-id="e4d91-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4d91-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e4d91-133">displayName</span></span>|<span data-ttu-id="e4d91-134">String</span><span class="sxs-lookup"><span data-stu-id="e4d91-134">String</span></span>|<span data-ttu-id="e4d91-135">Отображаемое имя папки.</span><span class="sxs-lookup"><span data-stu-id="e4d91-135">The folder's display name.</span></span>|
|<span data-ttu-id="e4d91-136">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="e4d91-136">parentFolderId</span></span>|<span data-ttu-id="e4d91-137">String</span><span class="sxs-lookup"><span data-stu-id="e4d91-137">String</span></span>|<span data-ttu-id="e4d91-138">Идентификатор родительской папки для папки.</span><span class="sxs-lookup"><span data-stu-id="e4d91-138">The ID of the folder's parent folder.</span></span>|
|<span data-ttu-id="e4d91-139">wellKnownName</span><span class="sxs-lookup"><span data-stu-id="e4d91-139">wellKnownName</span></span>|<span data-ttu-id="e4d91-140">string</span><span class="sxs-lookup"><span data-stu-id="e4d91-140">string</span></span>|<span data-ttu-id="e4d91-141">Имя папки, если она является распознаваемой папкой.</span><span class="sxs-lookup"><span data-stu-id="e4d91-141">The name of the folder if the folder is a recognized folder.</span></span> <span data-ttu-id="e4d91-142">В `contacts` настоящее время это единственная распознанная папка контактов.</span><span class="sxs-lookup"><span data-stu-id="e4d91-142">Currently `contacts` is the only recognized contacts folder.</span></span>|

## <a name="response"></a><span data-ttu-id="e4d91-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4d91-143">Response</span></span>

<span data-ttu-id="e4d91-144">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [contactFolder](../resources/contactfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e4d91-144">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/contactfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e4d91-145">Пример</span><span class="sxs-lookup"><span data-stu-id="e4d91-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e4d91-146">Запрос</span><span class="sxs-lookup"><span data-stu-id="e4d91-146">Request</span></span>
<span data-ttu-id="e4d91-147">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e4d91-147">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="e4d91-148">Отклик</span><span class="sxs-lookup"><span data-stu-id="e4d91-148">Response</span></span>
<span data-ttu-id="e4d91-p106">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e4d91-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e4d91-152">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="e4d91-152">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e4d91-153">C#</span><span class="sxs-lookup"><span data-stu-id="e4d91-153">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_contactfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e4d91-154">Javascript</span><span class="sxs-lookup"><span data-stu-id="e4d91-154">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_contactfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="e4d91-155">Цель — C</span><span class="sxs-lookup"><span data-stu-id="e4d91-155">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_contactfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/contactfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
