---
title: Удаление объекта contactFolder
description: Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.
ms.openlocfilehash: f2f7bfe8ceb396bd7ec034905d8655d0b6c0aefb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27028170"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="2d8b4-103">Удаление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="2d8b4-103">Delete contactFolder</span></span>

<span data-ttu-id="2d8b4-104">Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="2d8b4-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2d8b4-105">Permissions</span></span>
<span data-ttu-id="2d8b4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2d8b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d8b4-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2d8b4-108">Permission type</span></span>      | <span data-ttu-id="2d8b4-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2d8b4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2d8b4-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2d8b4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2d8b4-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d8b4-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2d8b4-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2d8b4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2d8b4-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d8b4-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="2d8b4-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2d8b4-114">Application</span></span> | <span data-ttu-id="2d8b4-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2d8b4-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="2d8b4-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2d8b4-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="2d8b4-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2d8b4-117">Request headers</span></span>
| <span data-ttu-id="2d8b4-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2d8b4-118">Name</span></span>       | <span data-ttu-id="2d8b4-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2d8b4-119">Type</span></span> | <span data-ttu-id="2d8b4-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2d8b4-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2d8b4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d8b4-121">Authorization</span></span>  | <span data-ttu-id="2d8b4-122">string</span><span class="sxs-lookup"><span data-stu-id="2d8b4-122">string</span></span>  | <span data-ttu-id="2d8b4-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2d8b4-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="2d8b4-125">Request body</span></span>
<span data-ttu-id="2d8b4-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2d8b4-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="2d8b4-127">Response</span></span>

<span data-ttu-id="2d8b4-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d8b4-130">Пример</span><span class="sxs-lookup"><span data-stu-id="2d8b4-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2d8b4-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="2d8b4-131">Request</span></span>
<span data-ttu-id="2d8b4-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="2d8b4-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="2d8b4-133">Response</span></span>
<span data-ttu-id="2d8b4-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="2d8b4-134">Here is an example of the response.</span></span> 
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
  "description": "Delete contactFolder",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
