---
title: Обновление объекта MailFolder
description: Обновление свойств объекта MailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 32bc67d56ecddbce1e0398ba26e7a9d162e3841e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274979"
---
# <a name="update-mailfolder"></a><span data-ttu-id="076e5-103">Обновление объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="076e5-103">Update mailfolder</span></span>

<span data-ttu-id="076e5-104">Обновление свойств объекта MailFolder.</span><span class="sxs-lookup"><span data-stu-id="076e5-104">Update the properties of mailfolder object.</span></span>
## <a name="permissions"></a><span data-ttu-id="076e5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="076e5-105">Permissions</span></span>
<span data-ttu-id="076e5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="076e5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="076e5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="076e5-108">Permission type</span></span>      | <span data-ttu-id="076e5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="076e5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="076e5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="076e5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="076e5-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="076e5-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="076e5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="076e5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="076e5-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="076e5-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="076e5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="076e5-114">Application</span></span> | <span data-ttu-id="076e5-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="076e5-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="076e5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="076e5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/mailFolders/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="076e5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="076e5-117">Request headers</span></span>
| <span data-ttu-id="076e5-118">Заголовок</span><span class="sxs-lookup"><span data-stu-id="076e5-118">Header</span></span>       | <span data-ttu-id="076e5-119">Значение</span><span class="sxs-lookup"><span data-stu-id="076e5-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="076e5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="076e5-120">Authorization</span></span>  | <span data-ttu-id="076e5-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="076e5-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="076e5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="076e5-123">Content-Type</span></span>  | <span data-ttu-id="076e5-p103">application/json. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="076e5-p103">application/json. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="076e5-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="076e5-126">Request body</span></span>
<span data-ttu-id="076e5-p104">В тексте запроса укажите значения для соответствующих полей, которые необходимо обновить. Предыдущие значения существующих свойств, не включенных в текст запроса, останутся прежними или будут повторно вычислены с учетом измененных значений других свойств. Для достижения оптимальной производительности не следует включать существующие значения, которые не изменились.</span><span class="sxs-lookup"><span data-stu-id="076e5-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="076e5-130">Свойство</span><span class="sxs-lookup"><span data-stu-id="076e5-130">Property</span></span>     | <span data-ttu-id="076e5-131">Тип</span><span class="sxs-lookup"><span data-stu-id="076e5-131">Type</span></span>   |<span data-ttu-id="076e5-132">Описание</span><span class="sxs-lookup"><span data-stu-id="076e5-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="076e5-133">displayName</span><span class="sxs-lookup"><span data-stu-id="076e5-133">displayName</span></span>|<span data-ttu-id="076e5-134">Строка</span><span class="sxs-lookup"><span data-stu-id="076e5-134">String</span></span>|<span data-ttu-id="076e5-135">Отображаемое имя элемента mailFolder.</span><span class="sxs-lookup"><span data-stu-id="076e5-135">The mailFolder's display name.</span></span>|

## <a name="response"></a><span data-ttu-id="076e5-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="076e5-136">Response</span></span>

<span data-ttu-id="076e5-137">В случае успеха этот метод возвращает код отклика `200 OK` и обновленный объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="076e5-137">If successful, this method returns a `200 OK` response code and updated [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="076e5-138">Пример</span><span class="sxs-lookup"><span data-stu-id="076e5-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="076e5-139">Запрос</span><span class="sxs-lookup"><span data-stu-id="076e5-139">Request</span></span>
<span data-ttu-id="076e5-140">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="076e5-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_mailfolder"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/mailFolders/{id}
Content-type: application/json
Content-length: 159

{
  "displayName": "displayName-value",
}
```
##### <a name="response"></a><span data-ttu-id="076e5-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="076e5-141">Response</span></span>
<span data-ttu-id="076e5-p105">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="076e5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "displayName": "displayName-value",
  "parentFolderId": "parentFolderId-value",
  "childFolderCount": 99,
  "unreadItemCount": 99,
  "totalItemCount": 99,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="076e5-145">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="076e5-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="076e5-146">C#</span><span class="sxs-lookup"><span data-stu-id="076e5-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="076e5-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="076e5-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="076e5-148">Цель — C</span><span class="sxs-lookup"><span data-stu-id="076e5-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update mailfolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
