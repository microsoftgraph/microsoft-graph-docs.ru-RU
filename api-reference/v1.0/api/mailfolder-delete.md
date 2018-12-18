---
title: Удаление объекта MailFolder
description: Удаление указанного mailFolder.
author: angelgolfer-ms
ms.openlocfilehash: ea2edfe07554ef0a5e1144dd1aeed00b7dd46155
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301101"
---
# <a name="delete-mailfolder"></a><span data-ttu-id="1ecfa-103">Удаление объекта MailFolder</span><span class="sxs-lookup"><span data-stu-id="1ecfa-103">Delete mailFolder</span></span>

<span data-ttu-id="1ecfa-104">Удаление указанного [mailFolder](../resources/mailfolder.md).</span><span class="sxs-lookup"><span data-stu-id="1ecfa-104">Delete the specified [mailFolder](../resources/mailfolder.md).</span></span>

<span data-ttu-id="1ecfa-105">Можно указать папку почты по Идентификатору папки или по его [имени известных папки](../resources/mailfolder.md), если он существует.</span><span class="sxs-lookup"><span data-stu-id="1ecfa-105">You can specify a mail folder by its folder ID, or by its [well-known folder name](../resources/mailfolder.md), if one exists.</span></span> 

><span data-ttu-id="1ecfa-106">**Примечание** Можно не удалять элементы в папке восстанавливаемый удалений (представленное имя папки известных `recoverableitemsdeletions`).</span><span class="sxs-lookup"><span data-stu-id="1ecfa-106">**Note** You may not be able to delete items in the recoverable items deletions folder (represented by the well-known folder name `recoverableitemsdeletions`).</span></span> <span data-ttu-id="1ecfa-107">Для получения дополнительных сведений см [хранения удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) и [Очистка удаленных элементов](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) .</span><span class="sxs-lookup"><span data-stu-id="1ecfa-107">See [Deleted item retention](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/recoverable-items-folder#deleted-item-retention) and [Clean up deleted items](https://docs.microsoft.com/en-us/exchange/policy-and-compliance/recoverable-items-folder/clean-up-deleted-items) for more information.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ecfa-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1ecfa-108">Permissions</span></span>
<span data-ttu-id="1ecfa-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ecfa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ecfa-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1ecfa-111">Permission type</span></span>      | <span data-ttu-id="1ecfa-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1ecfa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ecfa-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1ecfa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1ecfa-114">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ecfa-114">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1ecfa-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1ecfa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ecfa-116">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ecfa-116">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="1ecfa-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1ecfa-117">Application</span></span> | <span data-ttu-id="1ecfa-118">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1ecfa-118">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ecfa-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1ecfa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/mailFolders/{id}
DELETE /users/{id | userPrincipalName}/mailFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="1ecfa-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1ecfa-120">Request headers</span></span>
| <span data-ttu-id="1ecfa-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1ecfa-121">Name</span></span>       | <span data-ttu-id="1ecfa-122">Тип</span><span class="sxs-lookup"><span data-stu-id="1ecfa-122">Type</span></span> | <span data-ttu-id="1ecfa-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1ecfa-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1ecfa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ecfa-124">Authorization</span></span>  | <span data-ttu-id="1ecfa-125">string</span><span class="sxs-lookup"><span data-stu-id="1ecfa-125">string</span></span>  | <span data-ttu-id="1ecfa-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="1ecfa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ecfa-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1ecfa-128">Request body</span></span>
<span data-ttu-id="1ecfa-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1ecfa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ecfa-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="1ecfa-130">Response</span></span>

<span data-ttu-id="1ecfa-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="1ecfa-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ecfa-133">Пример</span><span class="sxs-lookup"><span data-stu-id="1ecfa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ecfa-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="1ecfa-134">Request</span></span>
<span data-ttu-id="1ecfa-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1ecfa-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_mailfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/mailFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="1ecfa-136">Ответ</span><span class="sxs-lookup"><span data-stu-id="1ecfa-136">Response</span></span>
<span data-ttu-id="1ecfa-137">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="1ecfa-137">Here is an example of the response.</span></span> 
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