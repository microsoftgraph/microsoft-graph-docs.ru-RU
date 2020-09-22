---
title: Удаление объекта MailFolder
description: Удаление указанного mailFolder или Маилсеарчфолдер.
author: svpsiva
localization_priority: Normal
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: e30fc8381b11534f88f265722609721cec364998
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076955"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="91421-103">Удаление объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="91421-103">Delete mailFolder</span></span>

<span data-ttu-id="91421-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91421-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91421-105">Удаление указанного [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="91421-105">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span> <span data-ttu-id="91421-106">Папка может быть [маилсеарчфолдер](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="91421-106">The folder can be a [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="91421-107">Вы можете указать почтовую папку по ее ИДЕНТИФИКАТОРу папки или по [известному имени папки](../resources/mailfolder.md), если она существует.</span><span class="sxs-lookup"><span data-stu-id="91421-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span>

><span data-ttu-id="91421-108">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным именем папки `recoverableitemsdeletions` ).</span><span class="sxs-lookup"><span data-stu-id="91421-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="91421-109">Дополнительные сведения см. в статье [Хранение удаленных](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="91421-109">See [Deleted item retention](/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="91421-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="91421-110">Permissions</span></span>
<span data-ttu-id="91421-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="91421-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91421-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="91421-113">Permission type</span></span>      | <span data-ttu-id="91421-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="91421-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91421-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="91421-115">Delegated (work or school account)</span></span> | <span data-ttu-id="91421-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91421-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="91421-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="91421-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91421-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91421-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="91421-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="91421-119">Application</span></span> | <span data-ttu-id="91421-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91421-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="91421-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="91421-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="91421-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="91421-122">Request headers</span></span>
| <span data-ttu-id="91421-123">Имя</span><span class="sxs-lookup"><span data-stu-id="91421-123">Name</span></span>       | <span data-ttu-id="91421-124">Тип</span><span class="sxs-lookup"><span data-stu-id="91421-124">Type</span></span> | <span data-ttu-id="91421-125">Описание</span><span class="sxs-lookup"><span data-stu-id="91421-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="91421-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="91421-126">Authorization</span></span>  | <span data-ttu-id="91421-127">string</span><span class="sxs-lookup"><span data-stu-id="91421-127">string</span></span>  | <span data-ttu-id="91421-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="91421-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91421-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="91421-130">Request body</span></span>
<span data-ttu-id="91421-131">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="91421-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="91421-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="91421-132">Response</span></span>
<span data-ttu-id="91421-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="91421-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91421-135">Пример</span><span class="sxs-lookup"><span data-stu-id="91421-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="91421-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="91421-136">Request</span></span>
<span data-ttu-id="91421-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="91421-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91421-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="91421-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```
# <a name="c"></a>[<span data-ttu-id="91421-139">C#</span><span class="sxs-lookup"><span data-stu-id="91421-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-mailfolder-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="91421-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91421-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-mailfolder-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="91421-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91421-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-mailfolder-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="91421-142">Отклик</span><span class="sxs-lookup"><span data-stu-id="91421-142">Response</span></span>
<span data-ttu-id="91421-143">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="91421-143">The following is an example of the response.</span></span>
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


