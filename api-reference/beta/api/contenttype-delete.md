---
author: swapnil1993
title: Удаление contentType
description: Удаление типа контента из списка sharepoint или сайта.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 8c27cfd2e16fc4c3bd7fade3f5546c08951f38c5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447274"
---
# <a name="delete-contenttype"></a><span data-ttu-id="0bc9d-103">Удаление contentType</span><span class="sxs-lookup"><span data-stu-id="0bc9d-103">Delete contentType</span></span>
<span data-ttu-id="0bc9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bc9d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0bc9d-105">Удаление [типа контента][contentType] из [списка][] или [сайта.][]</span><span class="sxs-lookup"><span data-stu-id="0bc9d-105">Remove a [content type][contentType] from a [list][] or a [site][].</span></span>


## <a name="permissions"></a><span data-ttu-id="0bc9d-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0bc9d-106">Permissions</span></span>
<span data-ttu-id="0bc9d-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0bc9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="0bc9d-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0bc9d-109">Permission type</span></span>      | <span data-ttu-id="0bc9d-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0bc9d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0bc9d-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0bc9d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0bc9d-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0bc9d-112">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span>    |
|<span data-ttu-id="0bc9d-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0bc9d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0bc9d-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0bc9d-114">Not supported.</span></span>    |
|<span data-ttu-id="0bc9d-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0bc9d-115">Application</span></span> | <span data-ttu-id="0bc9d-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0bc9d-116">Sites.ReadWrite.All, Sites.Manage.All, Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0bc9d-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0bc9d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /sites/{site-id}/contentTypes/{contentType-id}
DELETE /sites/{site-id}/lists/{list-id}/contentTypes/{contentType-id}
```

## <a name="request-headers"></a><span data-ttu-id="0bc9d-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0bc9d-118">Request headers</span></span>
|<span data-ttu-id="0bc9d-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0bc9d-119">Name</span></span>|<span data-ttu-id="0bc9d-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0bc9d-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0bc9d-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0bc9d-121">Authorization</span></span>|<span data-ttu-id="0bc9d-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0bc9d-p102">Bearer {token}. Required.</span></span>|


## <a name="request-body"></a><span data-ttu-id="0bc9d-124">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0bc9d-124">Request body</span></span>

<span data-ttu-id="0bc9d-125">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0bc9d-125">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bc9d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bc9d-126">Response</span></span>

<span data-ttu-id="0bc9d-127">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="0bc9d-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="0bc9d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="0bc9d-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="0bc9d-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0bc9d-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_contenttype"
}
-->

```http
DELETE https://graph.microsoft.com/beta/sites/{site-id}/contentTypes/{contentType-id}
```

### <a name="response"></a><span data-ttu-id="0bc9d-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="0bc9d-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->

```http
HTTP/1.1 204 No Content
```

[list]: ../resources/list.md
[contentType]: ../resources/contentType.md
[site]: ../resources/site.md
