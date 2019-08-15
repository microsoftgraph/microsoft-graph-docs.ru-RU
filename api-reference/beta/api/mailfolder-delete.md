---
title: Удаление объекта MailFolder
description: Удаление указанного mailFolder или Маилсеарчфолдер.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 190b80b1c707d1bffc87288a09356eff794d38c0
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/15/2019
ms.locfileid: "36415346"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="241a7-103">Удаление объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="241a7-103">Delete mailFolder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="241a7-104">Удаление указанного [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="241a7-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="241a7-105">Папка может быть [маилсеарчфолдер](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="241a7-105">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="241a7-106">Вы можете указать почтовую папку по ее ИДЕНТИФИКАТОРу папки или по известному [имени папки](../resources/mailfolder.md), если она существует.</span><span class="sxs-lookup"><span data-stu-id="241a7-106">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="241a7-107">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным именем `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="241a7-107">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="241a7-108">Дополнительные сведения см. в статье [Хранение удаленных](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="241a7-108">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="241a7-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="241a7-109">Permissions</span></span>
<span data-ttu-id="241a7-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="241a7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="241a7-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="241a7-112">Permission type</span></span>      | <span data-ttu-id="241a7-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="241a7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="241a7-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="241a7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="241a7-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="241a7-115">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="241a7-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="241a7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="241a7-117">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="241a7-117">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="241a7-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="241a7-118">Application</span></span> | <span data-ttu-id="241a7-119">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="241a7-119">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="241a7-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="241a7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="241a7-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="241a7-121">Request headers</span></span>
| <span data-ttu-id="241a7-122">Имя</span><span class="sxs-lookup"><span data-stu-id="241a7-122">Name</span></span>       | <span data-ttu-id="241a7-123">Тип</span><span class="sxs-lookup"><span data-stu-id="241a7-123">Type</span></span> | <span data-ttu-id="241a7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="241a7-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="241a7-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="241a7-125">Authorization</span></span>  | <span data-ttu-id="241a7-126">string</span><span class="sxs-lookup"><span data-stu-id="241a7-126">string</span></span>  | <span data-ttu-id="241a7-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="241a7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="241a7-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="241a7-129">Request body</span></span>
<span data-ttu-id="241a7-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="241a7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="241a7-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="241a7-131">Response</span></span>
<span data-ttu-id="241a7-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="241a7-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="241a7-134">Пример</span><span class="sxs-lookup"><span data-stu-id="241a7-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="241a7-135">Запрос</span><span class="sxs-lookup"><span data-stu-id="241a7-135">Request</span></span>
<span data-ttu-id="241a7-136">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="241a7-136">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="241a7-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="241a7-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="241a7-138">C#</span><span class="sxs-lookup"><span data-stu-id="241a7-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="241a7-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="241a7-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="241a7-140">Цель — C</span><span class="sxs-lookup"><span data-stu-id="241a7-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="241a7-141">Отклик</span><span class="sxs-lookup"><span data-stu-id="241a7-141">Response</span></span>
<span data-ttu-id="241a7-142">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="241a7-142">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
