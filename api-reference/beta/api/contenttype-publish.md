---
author: swapnil1993
title: 'contentType: публикация'
description: Публикация типа контента, присутствуют на сайте концентратора типов контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 072fb067114f9693f18a63c2d1e881fa55a7ca6b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447221"
---
# <a name="contenttype-publish"></a><span data-ttu-id="33b6f-103">contentType: публикация</span><span class="sxs-lookup"><span data-stu-id="33b6f-103">contentType: publish</span></span>
<span data-ttu-id="33b6f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33b6f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="33b6f-105">Публикует [контентТип,][] присутствующий на сайте концентратора типов контента.</span><span class="sxs-lookup"><span data-stu-id="33b6f-105">Publishes a [contentType][] present in content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="33b6f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="33b6f-106">Permissions</span></span>

<span data-ttu-id="33b6f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="33b6f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference.md).</span></span>

|<span data-ttu-id="33b6f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="33b6f-109">Permission type</span></span>      | <span data-ttu-id="33b6f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="33b6f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33b6f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="33b6f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33b6f-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="33b6f-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="33b6f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="33b6f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33b6f-114">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="33b6f-114">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="33b6f-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="33b6f-115">Application</span></span> | <span data-ttu-id="33b6f-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="33b6f-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33b6f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="33b6f-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
```http
POST /sites/{siteId}/contentTypes/{contentTypeId}/publish
```

><span data-ttu-id="33b6f-118">**Примечание:** SiteId представляет веб-узел типа контента.</span><span class="sxs-lookup"><span data-stu-id="33b6f-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33b6f-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="33b6f-119">Request headers</span></span>
|<span data-ttu-id="33b6f-120">Имя</span><span class="sxs-lookup"><span data-stu-id="33b6f-120">Name</span></span>|<span data-ttu-id="33b6f-121">Описание</span><span class="sxs-lookup"><span data-stu-id="33b6f-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="33b6f-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="33b6f-122">Authorization</span></span>|<span data-ttu-id="33b6f-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="33b6f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="33b6f-125">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="33b6f-125">Request body</span></span>
<span data-ttu-id="33b6f-126">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="33b6f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33b6f-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="33b6f-127">Response</span></span>
<span data-ttu-id="33b6f-128">В случае успешного ответа этот вызов возвращает `204 No Content` ответ.</span><span class="sxs-lookup"><span data-stu-id="33b6f-128">If successful, this call returns a `204 No Content` response.</span></span>

## <a name="example"></a><span data-ttu-id="33b6f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="33b6f-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="33b6f-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="33b6f-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_publish"
}
-->
```http
POST https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/publish
```

### <a name="response"></a><span data-ttu-id="33b6f-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="33b6f-131">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[contentType]: ../resources/contentType.md
