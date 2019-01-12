---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: Удаление записи из списка SharePoint
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1b61c9359ca349a7f7882a204e8e474aba00444b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968465"
---
# <a name="delete-an-item-from-a-list"></a><span data-ttu-id="1755e-102">Удаление элемента из списка</span><span class="sxs-lookup"><span data-stu-id="1755e-102">Delete an item from a list</span></span>

> <span data-ttu-id="1755e-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1755e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1755e-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1755e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1755e-105">Удаление элемента из [списка][].</span><span class="sxs-lookup"><span data-stu-id="1755e-105">Removes an item from a [list][].</span></span>

[list]: ../resources/list.md

## <a name="permissions"></a><span data-ttu-id="1755e-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1755e-107">Permissions</span></span>

<span data-ttu-id="1755e-108">Чтобы можно было удалить элемент, пользователь должен предоставить приложению доступ на запись к элементу, который необходимо удалить.</span><span class="sxs-lookup"><span data-stu-id="1755e-108">To delete an item, the user must have granted the application write access to the item to be deleted.</span></span>

<span data-ttu-id="1755e-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1755e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1755e-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1755e-111">Permission type</span></span>      | <span data-ttu-id="1755e-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1755e-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1755e-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1755e-113">Delegated (work or school account)</span></span> | <span data-ttu-id="1755e-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1755e-114">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1755e-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1755e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1755e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1755e-116">Not supported.</span></span>    |
|<span data-ttu-id="1755e-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1755e-117">Application</span></span> | <span data-ttu-id="1755e-118">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1755e-118">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1755e-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1755e-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="1755e-120">Необязательные заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1755e-120">Optional request headers</span></span>

| <span data-ttu-id="1755e-121">Имя</span><span class="sxs-lookup"><span data-stu-id="1755e-121">Name</span></span>       | <span data-ttu-id="1755e-122">Значение</span><span class="sxs-lookup"><span data-stu-id="1755e-122">Value</span></span> | <span data-ttu-id="1755e-123">Описание</span><span class="sxs-lookup"><span data-stu-id="1755e-123">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="1755e-124">_if-match_</span><span class="sxs-lookup"><span data-stu-id="1755e-124">_if-match_</span></span> | <span data-ttu-id="1755e-125">etag</span><span class="sxs-lookup"><span data-stu-id="1755e-125">etag</span></span>  | <span data-ttu-id="1755e-126">Если указан этот заголовок запроса, а предоставленный тег eTag не совпадает с текущим тегом элемента, то будет возвращен ответ `412 Precondition Failed`, и элемент не будет удален.</span><span class="sxs-lookup"><span data-stu-id="1755e-126">If this request header is included and the eTag provided does not match the current tag on the item, a `412 Precondition Failed` response is returned and the item will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="1755e-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="1755e-127">Request body</span></span>

<span data-ttu-id="1755e-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="1755e-128">Do not supply a request body with this method.</span></span>

## <a name="example"></a><span data-ttu-id="1755e-129">Пример</span><span class="sxs-lookup"><span data-stu-id="1755e-129">Example</span></span>

<!-- { "blockType": "request", "name": "delete-item", "scopes": "files.readwrite" } -->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}
```

## <a name="response"></a><span data-ttu-id="1755e-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="1755e-130">Response</span></span>

<span data-ttu-id="1755e-131">В случае успешного запроса этот вызов возвращает отклик `204 No Content`, указывающий, что ресурс удален, поэтому данные не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="1755e-131">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

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
