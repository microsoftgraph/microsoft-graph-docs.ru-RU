---
title: Получение объекта mailFolder
description: Получение свойств и связей объекта папки сообщений.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 010e6f0ada9de12655a5ebed341b5bbfdb26e124
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612676"
---
# <a name="get-mailfolder"></a><span data-ttu-id="409d3-103">Получение объекта mailFolder</span><span class="sxs-lookup"><span data-stu-id="409d3-103">Get mailFolder</span></span>

<span data-ttu-id="409d3-104">Получение свойств и связей объекта папки сообщений.</span><span class="sxs-lookup"><span data-stu-id="409d3-104">Retrieve the properties and relationships of a message folder object.</span></span>

<span data-ttu-id="409d3-105">Существует два сценария, в которых приложение может получить папку почты другого пользователя:</span><span class="sxs-lookup"><span data-stu-id="409d3-105">There are two scenarios where an app can get another user's mail folder:</span></span>

* <span data-ttu-id="409d3-106">У приложения есть разрешения для приложений; или</span><span class="sxs-lookup"><span data-stu-id="409d3-106">If the app has application permissions, or,</span></span>
* <span data-ttu-id="409d3-107">У приложения есть соответствующие делегированные [разрешения](#permissions) от одного пользователя, а другой пользователь поделился с ним папкой почты или предоставил ему делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="409d3-107">If the app has the appropriate delegated [permissions](#permissions) from one user, and another user has shared a mail folder with that user, or, has given delegated access to that user.</span></span> <span data-ttu-id="409d3-108">См. [подробные сведения и пример](/graph/outlook-share-messages-folders).</span><span class="sxs-lookup"><span data-stu-id="409d3-108">See [details and an example](/graph/outlook-share-messages-folders).</span></span>


## <a name="permissions"></a><span data-ttu-id="409d3-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="409d3-109">Permissions</span></span>
<span data-ttu-id="409d3-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="409d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="409d3-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="409d3-112">Permission type</span></span>      | <span data-ttu-id="409d3-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="409d3-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="409d3-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="409d3-114">Delegated (work or school account)</span></span> | <span data-ttu-id="409d3-115">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="409d3-115">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="409d3-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="409d3-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="409d3-117">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="409d3-117">Mail.Read, Mail.ReadWrite</span></span>    |
|<span data-ttu-id="409d3-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="409d3-118">Application</span></span> | <span data-ttu-id="409d3-119">Mail.Read, Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="409d3-119">Mail.Read, Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="409d3-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="409d3-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/mailFolders/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="409d3-121">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="409d3-121">Optional query parameters</span></span>
<span data-ttu-id="409d3-122">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="409d3-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="409d3-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="409d3-123">Request headers</span></span>
| <span data-ttu-id="409d3-124">Имя</span><span class="sxs-lookup"><span data-stu-id="409d3-124">Name</span></span>       | <span data-ttu-id="409d3-125">Тип</span><span class="sxs-lookup"><span data-stu-id="409d3-125">Type</span></span> | <span data-ttu-id="409d3-126">Описание</span><span class="sxs-lookup"><span data-stu-id="409d3-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="409d3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="409d3-127">Authorization</span></span>  | <span data-ttu-id="409d3-128">string</span><span class="sxs-lookup"><span data-stu-id="409d3-128">string</span></span>  | <span data-ttu-id="409d3-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="409d3-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="409d3-131">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="409d3-131">Request body</span></span>
<span data-ttu-id="409d3-132">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="409d3-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="409d3-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="409d3-133">Response</span></span>

<span data-ttu-id="409d3-134">В случае успеха этот метод возвращает код отклика `200 OK` и объект [mailFolder](../resources/mailfolder.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="409d3-134">If successful, this method returns a `200 OK` response code and [mailFolder](../resources/mailfolder.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="409d3-135">Пример</span><span class="sxs-lookup"><span data-stu-id="409d3-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="409d3-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="409d3-136">Request</span></span>
<span data-ttu-id="409d3-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="409d3-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_mailfolder"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="409d3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="409d3-138">Response</span></span>
<span data-ttu-id="409d3-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="409d3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="409d3-142">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="409d3-142">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="409d3-143">C#</span><span class="sxs-lookup"><span data-stu-id="409d3-143">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="409d3-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="409d3-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
