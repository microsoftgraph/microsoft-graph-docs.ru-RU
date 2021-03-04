---
author: swapnil1993
title: 'contentType: неопубликованный'
description: Отопубликуй тип контента с сайта концентратора типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: ca432973337ac81f3ee8e632bb0705f26c7575ea
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447218"
---
# <a name="contenttype-unpublish"></a><span data-ttu-id="a00cf-103">contentType: неопубликованный</span><span class="sxs-lookup"><span data-stu-id="a00cf-103">contentType: unpublish</span></span>
<span data-ttu-id="a00cf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a00cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="a00cf-105">Unpublish a [contentType][] from a content type hub site.</span><span class="sxs-lookup"><span data-stu-id="a00cf-105">Unpublish a [contentType][] from a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="a00cf-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a00cf-106">Permissions</span></span>

<span data-ttu-id="a00cf-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a00cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="a00cf-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a00cf-109">Permission type</span></span>      | <span data-ttu-id="a00cf-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a00cf-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a00cf-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a00cf-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a00cf-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a00cf-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="a00cf-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a00cf-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a00cf-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a00cf-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="a00cf-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="a00cf-115">Application</span></span> | <span data-ttu-id="a00cf-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a00cf-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a00cf-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a00cf-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

><span data-ttu-id="a00cf-118">**Примечание:** SiteId представляет веб-узел типа контента.</span><span class="sxs-lookup"><span data-stu-id="a00cf-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a00cf-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a00cf-119">Request headers</span></span>
|<span data-ttu-id="a00cf-120">Имя</span><span class="sxs-lookup"><span data-stu-id="a00cf-120">Name</span></span>|<span data-ttu-id="a00cf-121">Описание</span><span class="sxs-lookup"><span data-stu-id="a00cf-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a00cf-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a00cf-122">Authorization</span></span>|<span data-ttu-id="a00cf-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a00cf-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a00cf-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="a00cf-125">Request body</span></span>
<span data-ttu-id="a00cf-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a00cf-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a00cf-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="a00cf-127">Response</span></span>

<span data-ttu-id="a00cf-128">В случае успешной работы этот метод возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="a00cf-128">If successful, this method returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="a00cf-129">Пример</span><span class="sxs-lookup"><span data-stu-id="a00cf-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a00cf-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="a00cf-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_unpublish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/unpublish
```

### <a name="response"></a><span data-ttu-id="a00cf-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a00cf-131">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
