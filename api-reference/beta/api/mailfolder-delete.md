---
title: Удаление объекта MailFolder
description: Удаление указанного mailFolder или mailSearchFolder.
ms.openlocfilehash: 4b1a79a871ebf03656fa33474480e7169943e035
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078435"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="a302b-103">Удаление объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="a302b-103">Delete mailFolder</span></span>

> <span data-ttu-id="a302b-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="a302b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a302b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a302b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a302b-106">Удаление указанного [mailFolder](../resources/mailfolder.md) или [mailSearchFolder](../resources/mailsearchfolder.md).</span><span class="sxs-lookup"><span data-stu-id="a302b-106">Delete the specified [mailFolder](../resources/mailfolder.md) or [mailSearchFolder](../resources/mailsearchfolder.md).</span></span>

<span data-ttu-id="a302b-107">Можно указать папку почты по Идентификатору папки или по его [имени известных папки](../resources/mailfolder.md), если он существует.</span><span class="sxs-lookup"><span data-stu-id="a302b-107">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="a302b-108">**Примечание** Можно не удалять элементы в папке восстанавливаемый удалений (представленное имя папки известных `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="a302b-108">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="a302b-109">Для получения дополнительных сведений см [хранения удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="a302b-109">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="a302b-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a302b-110">Permissions</span></span>
<span data-ttu-id="a302b-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a302b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a302b-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a302b-113">Permission type</span></span>      | <span data-ttu-id="a302b-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a302b-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a302b-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a302b-115">Delegated (work or school account)</span></span> | <span data-ttu-id="a302b-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a302b-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a302b-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a302b-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a302b-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a302b-118">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="a302b-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a302b-119">Application</span></span> | <span data-ttu-id="a302b-120">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a302b-120">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="a302b-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a302b-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a302b-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a302b-122">Request headers</span></span>
| <span data-ttu-id="a302b-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a302b-123">Name</span></span>       | <span data-ttu-id="a302b-124">Тип</span><span class="sxs-lookup"><span data-stu-id="a302b-124">Type</span></span> | <span data-ttu-id="a302b-125">Описание</span><span class="sxs-lookup"><span data-stu-id="a302b-125">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a302b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a302b-126">Authorization</span></span>  | <span data-ttu-id="a302b-127">string</span><span class="sxs-lookup"><span data-stu-id="a302b-127">string</span></span>  | <span data-ttu-id="a302b-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a302b-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a302b-130">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a302b-130">Request body</span></span>
<span data-ttu-id="a302b-131">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a302b-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a302b-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="a302b-132">Response</span></span>
<span data-ttu-id="a302b-p105">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a302b-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a302b-135">Пример</span><span class="sxs-lookup"><span data-stu-id="a302b-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="a302b-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="a302b-136">Request</span></span>
<span data-ttu-id="a302b-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a302b-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/beta/me/mailFolders/AAMkAGVmMDEzM/
```

#### <a name="response"></a><span data-ttu-id="a302b-138">Ответ</span><span class="sxs-lookup"><span data-stu-id="a302b-138">Response</span></span>
<span data-ttu-id="a302b-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="a302b-139">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete mailFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->