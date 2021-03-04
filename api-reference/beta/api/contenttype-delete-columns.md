---
author: swapnil1993
title: Удаление columnDefinition
description: Удаление столбца из типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: fb5df6389c4723cf48185a74f72c1009a3ac031b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447279"
---
# <a name="delete-columndefinition"></a><span data-ttu-id="929d7-103">Удаление columnDefinition</span><span class="sxs-lookup"><span data-stu-id="929d7-103">Delete columnDefinition</span></span>
<span data-ttu-id="929d7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="929d7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="929d7-105">Удаление [столбца][columndefinition] из [списка][] или типа [контента][] [сайта.][contentType]</span><span class="sxs-lookup"><span data-stu-id="929d7-105">Remove a [column][columndefinition] from a [list][] or a [site][] [content type][contentType].</span></span>


## <a name="permissions"></a><span data-ttu-id="929d7-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="929d7-106">Permissions</span></span>
<span data-ttu-id="929d7-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="929d7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="929d7-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="929d7-109">Permission type</span></span>      | <span data-ttu-id="929d7-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="929d7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="929d7-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="929d7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="929d7-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="929d7-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="929d7-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="929d7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="929d7-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="929d7-114">Not supported.</span></span>    |
|<span data-ttu-id="929d7-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="929d7-115">Application</span></span> | <span data-ttu-id="929d7-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="929d7-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="929d7-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="929d7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}/columns/{column-id}
```
## <a name="request-headers"></a><span data-ttu-id="929d7-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="929d7-118">Request headers</span></span>
|<span data-ttu-id="929d7-119">Имя</span><span class="sxs-lookup"><span data-stu-id="929d7-119">Name</span></span>|<span data-ttu-id="929d7-120">Описание</span><span class="sxs-lookup"><span data-stu-id="929d7-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="929d7-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="929d7-121">Authorization</span></span>|<span data-ttu-id="929d7-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="929d7-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="929d7-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="929d7-124">Request body</span></span>
<span data-ttu-id="929d7-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="929d7-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="929d7-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="929d7-126">Response</span></span>

<span data-ttu-id="929d7-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="929d7-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="929d7-128">Пример</span><span class="sxs-lookup"><span data-stu-id="929d7-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="929d7-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="929d7-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_columns_from_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}/columns/{column-id}
```

### <a name="response"></a><span data-ttu-id="929d7-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="929d7-130">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[columndefinition]: ../resources/columndefinition.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
