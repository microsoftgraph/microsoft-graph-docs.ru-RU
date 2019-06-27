---
title: Удаление объекта MailFolder
description: Удаление указанного mailFolder или Маилсеарчфолдер.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d219d9c410573b932c7022b2aea50826d0a016c1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2019
ms.locfileid: "35266138"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="23baf-103">Удаление объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="23baf-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23baf-104">Удаление указанного [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="23baf-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="23baf-105">Папка может быть [маилсеарчфолдер](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="23baf-105">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="23baf-106">Вы можете указать почтовую папку по ее ИДЕНТИФИКАТОРу папки или по известному [имени папки](../resources/mailfolder.md), если она существует.</span><span class="sxs-lookup"><span data-stu-id="23baf-106">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="23baf-107">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным именем `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="23baf-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="23baf-108">Дополнительные сведения см. в статье [Хранение удаленных](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="23baf-108">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="23baf-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="23baf-109">Permissions</span></span>
<span data-ttu-id="23baf-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="23baf-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23baf-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="23baf-112">Permission type</span></span>      | <span data-ttu-id="23baf-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="23baf-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23baf-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="23baf-114">Delegated (work or school account)</span></span> | <span data-ttu-id="23baf-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23baf-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="23baf-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="23baf-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23baf-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23baf-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="23baf-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="23baf-118">Application</span></span> | <span data-ttu-id="23baf-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="23baf-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="23baf-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="23baf-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="23baf-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="23baf-121">Request headers</span></span>
| <span data-ttu-id="23baf-122">Имя</span><span class="sxs-lookup"><span data-stu-id="23baf-122">Name</span></span>       | <span data-ttu-id="23baf-123">Тип</span><span class="sxs-lookup"><span data-stu-id="23baf-123">Type</span></span> | <span data-ttu-id="23baf-124">Описание</span><span class="sxs-lookup"><span data-stu-id="23baf-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="23baf-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="23baf-125">Authorization</span></span>  | <span data-ttu-id="23baf-126">string</span><span class="sxs-lookup"><span data-stu-id="23baf-126">string</span></span>  | <span data-ttu-id="23baf-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="23baf-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="23baf-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="23baf-129">Request body</span></span>
<span data-ttu-id="23baf-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="23baf-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23baf-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="23baf-131">Response</span></span>
<span data-ttu-id="23baf-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="23baf-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23baf-134">Пример</span><span class="sxs-lookup"><span data-stu-id="23baf-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="23baf-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="23baf-135">Request</span></span>
<span data-ttu-id="23baf-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="23baf-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="23baf-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="23baf-137">Response</span></span>
<span data-ttu-id="23baf-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="23baf-138">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="23baf-139">Пример кода SDK</span><span class="sxs-lookup"><span data-stu-id="23baf-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="23baf-140">C#</span><span class="sxs-lookup"><span data-stu-id="23baf-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23baf-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="23baf-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="23baf-142">Цель — C</span><span class="sxs-lookup"><span data-stu-id="23baf-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
