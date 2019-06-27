---
title: Вывод ресурса
description: Получение двоичных данных объекта ресурса файла или изображения.
localization_priority: Normal
author: jewan-microsoft
ms.prod: onenote
ms.openlocfilehash: 06afaf3eedcb80e541dac1ba28514cd8f95869fb
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35265018"
---
# <a name="get-resource"></a><span data-ttu-id="90dce-103">Вывод ресурса</span><span class="sxs-lookup"><span data-stu-id="90dce-103">Get resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90dce-104">Получение двоичных данных объекта [ресурса](../resources/onenoteresource.md) файла или изображения.</span><span class="sxs-lookup"><span data-stu-id="90dce-104">Retrieve the binary data of a file or image [resource](../resources/onenoteresource.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="90dce-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="90dce-105">Permissions</span></span>
<span data-ttu-id="90dce-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90dce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90dce-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="90dce-108">Permission type</span></span>      | <span data-ttu-id="90dce-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="90dce-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="90dce-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="90dce-110">Delegated (work or school account)</span></span> | <span data-ttu-id="90dce-111">Notes. Read, Notes. ReadWrite, Notes. Read. ALL, Notes. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="90dce-111">Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="90dce-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="90dce-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="90dce-113">Notes. Read, Notes. ReadWrite</span><span class="sxs-lookup"><span data-stu-id="90dce-113">Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="90dce-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="90dce-114">Application</span></span> | <span data-ttu-id="90dce-115">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90dce-115">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="90dce-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="90dce-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/resources/{id}/content
GET /users/{id | userPrincipalName}/onenote/resources/{id}/content
GET /groups/{id}/onenote/resources/{id}/content
GET /sites/{id}/onenote/resources/{id}/content
```

## <a name="request-headers"></a><span data-ttu-id="90dce-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="90dce-117">Request headers</span></span>
| <span data-ttu-id="90dce-118">Имя</span><span class="sxs-lookup"><span data-stu-id="90dce-118">Name</span></span>       | <span data-ttu-id="90dce-119">Тип</span><span class="sxs-lookup"><span data-stu-id="90dce-119">Type</span></span> | <span data-ttu-id="90dce-120">Описание</span><span class="sxs-lookup"><span data-stu-id="90dce-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="90dce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="90dce-121">Authorization</span></span>  | <span data-ttu-id="90dce-122">string</span><span class="sxs-lookup"><span data-stu-id="90dce-122">string</span></span>  | <span data-ttu-id="90dce-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="90dce-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="90dce-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="90dce-125">Request body</span></span>
<span data-ttu-id="90dce-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="90dce-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90dce-127">Ответ</span><span class="sxs-lookup"><span data-stu-id="90dce-127">Response</span></span>

<span data-ttu-id="90dce-128">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и двоичные данные изображения или файла в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="90dce-128">If successful, this method returns a `200 OK` response code and the image or file binary data in the response body.</span></span>

<span data-ttu-id="90dce-129">Note: изображения не отображаются непосредственно в браузере, так как им требуется авторизация для их извлечения, как и остальная часть контента страницы.</span><span class="sxs-lookup"><span data-stu-id="90dce-129">Note: Images won't render directly in a browser because they require authorization to retrieve them, like the rest of the page content.</span></span>
## <a name="example"></a><span data-ttu-id="90dce-130">Пример</span><span class="sxs-lookup"><span data-stu-id="90dce-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="90dce-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="90dce-131">Request</span></span>
<span data-ttu-id="90dce-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="90dce-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_resource"
}-->
```http
GET https://graph.microsoft.com/beta/me/onenote/resources/{id}/content
```
##### <a name="response"></a><span data-ttu-id="90dce-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="90dce-133">Response</span></span>
<span data-ttu-id="90dce-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="90dce-134">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "stream"
} -->
```http
HTTP/1.1 200 OK
Content-Type: application/octet-stream

...binary data...
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="90dce-135">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="90dce-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="90dce-136">C#</span><span class="sxs-lookup"><span data-stu-id="90dce-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_resource-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="90dce-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="90dce-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_resource-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="90dce-138">Цель — C</span><span class="sxs-lookup"><span data-stu-id="90dce-138">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_resource-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/resource-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/resource-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/resource-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
