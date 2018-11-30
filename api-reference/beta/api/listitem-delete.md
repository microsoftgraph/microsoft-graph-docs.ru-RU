---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
ms.openlocfilehash: d0b39a7c0ca69d3bfdd0edb256ac20711dfe5efc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080382"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="ab05b-102">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="ab05b-102">Delete an item from a list</span></span>

> <span data-ttu-id="ab05b-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ab05b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab05b-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab05b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab05b-105">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="ab05b-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="ab05b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ab05b-107">Permissions</span></span>

<span data-ttu-id="ab05b-108">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="ab05b-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="ab05b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab05b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab05b-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ab05b-111">Permission type</span></span>      | <span data-ttu-id="ab05b-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ab05b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab05b-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ab05b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="ab05b-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab05b-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab05b-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ab05b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab05b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ab05b-116">Not supported.</span></span>    |
|<span data-ttu-id="ab05b-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ab05b-117">Application</span></span> | <span data-ttu-id="ab05b-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab05b-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab05b-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ab05b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ab05b-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ab05b-120">Optional request headers</span></span>

| <span data-ttu-id="ab05b-121">Имя</span><span class="sxs-lookup"><span data-stu-id="ab05b-121">Name</span></span>       | <span data-ttu-id="ab05b-122">Значение</span><span class="sxs-lookup"><span data-stu-id="ab05b-122">Value</span></span> | <span data-ttu-id="ab05b-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ab05b-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="ab05b-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="ab05b-124">_if-match_</span></span> | <span data-ttu-id="ab05b-125">etag</span><span class="sxs-lookup"><span data-stu-id="ab05b-125">etag</span></span>  | <span data-ttu-id="ab05b-126">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="ab05b-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="ab05b-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ab05b-127">Request body</span></span>

<span data-ttu-id="ab05b-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="ab05b-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="ab05b-129">Пример</span><span class="sxs-lookup"><span data-stu-id="ab05b-129">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="ab05b-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="ab05b-130">Response</span></span>

<span data-ttu-id="ab05b-131">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="ab05b-131">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Delete"
} -->
