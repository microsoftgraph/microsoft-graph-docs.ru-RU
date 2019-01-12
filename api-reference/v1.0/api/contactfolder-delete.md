---
title: Удаление объекта contactFolder
description: Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: f15cf3e08c01e7bf622fa17dd8ce59017ddb4f8c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976655"
---
# <a name="delete-contactfolder"></a><span data-ttu-id="9c2e6-103">Удаление объекта contactFolder</span><span class="sxs-lookup"><span data-stu-id="9c2e6-103">Delete contactFolder</span></span>

<span data-ttu-id="9c2e6-104">Удаление любого объекта contactFolder, кроме объекта contactFolder по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9c2e6-104">Delete contactFolder other than the default contactFolder.</span></span>
## <a name="permissions"></a><span data-ttu-id="9c2e6-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9c2e6-105">Permissions</span></span>
<span data-ttu-id="9c2e6-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c2e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c2e6-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9c2e6-108">Permission type</span></span>      | <span data-ttu-id="9c2e6-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9c2e6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9c2e6-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9c2e6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9c2e6-111">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c2e6-111">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9c2e6-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9c2e6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9c2e6-113">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c2e6-113">Contacts.ReadWrite</span></span>    |
|<span data-ttu-id="9c2e6-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9c2e6-114">Application</span></span> | <span data-ttu-id="9c2e6-115">Contacts.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="9c2e6-115">Contacts.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="9c2e6-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9c2e6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /me/contactFolders/{id}
DELETE /users/{id | userPrincipalName}/contactFolders/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9c2e6-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9c2e6-117">Request headers</span></span>
| <span data-ttu-id="9c2e6-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9c2e6-118">Name</span></span>       | <span data-ttu-id="9c2e6-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9c2e6-119">Type</span></span> | <span data-ttu-id="9c2e6-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9c2e6-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9c2e6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c2e6-121">Authorization</span></span>  | <span data-ttu-id="9c2e6-122">строка</span><span class="sxs-lookup"><span data-stu-id="9c2e6-122">string</span></span>  | <span data-ttu-id="9c2e6-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9c2e6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9c2e6-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="9c2e6-125">Request body</span></span>
<span data-ttu-id="9c2e6-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9c2e6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c2e6-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="9c2e6-127">Response</span></span>

<span data-ttu-id="9c2e6-p103">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="9c2e6-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c2e6-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9c2e6-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9c2e6-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9c2e6-131">Request</span></span>
<span data-ttu-id="9c2e6-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9c2e6-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contactfolder"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/me/contactFolders/{id}
```
##### <a name="response"></a><span data-ttu-id="9c2e6-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9c2e6-133">Response</span></span>
<span data-ttu-id="9c2e6-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="9c2e6-134">Here is an example of the response.</span></span> 
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
