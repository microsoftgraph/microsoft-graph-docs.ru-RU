---
title: Удаление объекта MailFolder
description: Удаление указанного mailFolder.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 1effb7d8e0ba6a27ddbef979f85c6e1e81adcecd
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2019
ms.locfileid: "33612648"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="ba5aa-103">Удаление объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="ba5aa-103">Delete mailFolder</span></span>

<span data-ttu-id="ba5aa-104">Удаление указанного [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="ba5aa-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="ba5aa-105">Вы можете указать почтовую папку по ее ИДЕНТИФИКАТОРу папки или по известному [имени папки](../resources/mailfolder.md), если она существует.</span><span class="sxs-lookup"><span data-stu-id="ba5aa-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="ba5aa-106">**Note (Примечание** ) Удаление элементов из папки "удаления элементов с возможностью восстановления" может быть недоступно (представлено известным именем `recoverableitemsdeletions`папки).</span><span class="sxs-lookup"><span data-stu-id="ba5aa-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="ba5aa-107">Дополнительные сведения см. в статье [Хранение удаленных](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) элементов и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="ba5aa-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="ba5aa-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ba5aa-108">Permissions</span></span>
<span data-ttu-id="ba5aa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ba5aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba5aa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ba5aa-111">Permission type</span></span>      | <span data-ttu-id="ba5aa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ba5aa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ba5aa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ba5aa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ba5aa-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba5aa-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ba5aa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ba5aa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ba5aa-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba5aa-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="ba5aa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ba5aa-117">Application</span></span> | <span data-ttu-id="ba5aa-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="ba5aa-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="ba5aa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ba5aa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="ba5aa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ba5aa-120">Request headers</span></span>
| <span data-ttu-id="ba5aa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ba5aa-121">Name</span></span>       | <span data-ttu-id="ba5aa-122">Тип</span><span class="sxs-lookup"><span data-stu-id="ba5aa-122">Type</span></span> | <span data-ttu-id="ba5aa-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ba5aa-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="ba5aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba5aa-124">Authorization</span></span>  | <span data-ttu-id="ba5aa-125">string</span><span class="sxs-lookup"><span data-stu-id="ba5aa-125">string</span></span>  | <span data-ttu-id="ba5aa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="ba5aa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ba5aa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ba5aa-128">Request body</span></span>
<span data-ttu-id="ba5aa-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ba5aa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba5aa-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ba5aa-130">Response</span></span>

<span data-ttu-id="ba5aa-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ba5aa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba5aa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="ba5aa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ba5aa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="ba5aa-134">Request</span></span>
<span data-ttu-id="ba5aa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ba5aa-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="ba5aa-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="ba5aa-136">Response</span></span>
<span data-ttu-id="ba5aa-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ba5aa-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ba5aa-138">Пример кода для SDK</span><span class="sxs-lookup"><span data-stu-id="ba5aa-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ba5aa-139">Языках</span><span class="sxs-lookup"><span data-stu-id="ba5aa-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ba5aa-140">Язык</span><span class="sxs-lookup"><span data-stu-id="ba5aa-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_mailfolder-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/mailfolder-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
