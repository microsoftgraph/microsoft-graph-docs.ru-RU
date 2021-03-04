---
author: swapnil1993
title: 'contentType: isPublished'
description: Проверьте состояние публикации типа контента на веб-узбе типа контента.
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: d6f5700015dcb69ce3440be187654941816e0a9d
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447250"
---
# <a name="contenttype-ispublished"></a><span data-ttu-id="0f483-103">contentType: isPublished</span><span class="sxs-lookup"><span data-stu-id="0f483-103">contentType: isPublished</span></span>
<span data-ttu-id="0f483-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f483-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="0f483-105">Проверьте состояние публикации [контентаType][] на веб-сайте концентратора типа контента.</span><span class="sxs-lookup"><span data-stu-id="0f483-105">Check the publishing status of a [contentType][] in a content type hub site.</span></span>

## <a name="permissions"></a><span data-ttu-id="0f483-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0f483-106">Permissions</span></span>

<span data-ttu-id="0f483-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0f483-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f483-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0f483-109">Permission type</span></span>      | <span data-ttu-id="0f483-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0f483-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0f483-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0f483-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0f483-112">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0f483-112">Sites.FullControl.All</span></span>    |
|<span data-ttu-id="0f483-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0f483-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0f483-114">Не поддерживается</span><span class="sxs-lookup"><span data-stu-id="0f483-114">Not Supported</span></span>   |
|<span data-ttu-id="0f483-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="0f483-115">Application</span></span> | <span data-ttu-id="0f483-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="0f483-116">Sites.FullControl.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0f483-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0f483-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
><span data-ttu-id="0f483-118">**Примечание:** SiteId представляет веб-узел типа контента.</span><span class="sxs-lookup"><span data-stu-id="0f483-118">**Note:** The siteId represents a content type hub site.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0f483-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0f483-119">Request headers</span></span>
|<span data-ttu-id="0f483-120">Имя</span><span class="sxs-lookup"><span data-stu-id="0f483-120">Name</span></span>|<span data-ttu-id="0f483-121">Описание</span><span class="sxs-lookup"><span data-stu-id="0f483-121">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0f483-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0f483-122">Authorization</span></span>|<span data-ttu-id="0f483-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0f483-p102">Bearer {token}. Required.</span></span>|

## <a name="response"></a><span data-ttu-id="0f483-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f483-125">Response</span></span>
<span data-ttu-id="0f483-126">В случае успешной работы этот вызов возвращает ответ и значение boolean, указывав состояние публикации `200 OK` типа контента.</span><span class="sxs-lookup"><span data-stu-id="0f483-126">If successful, this call returns a `200 OK` response and a boolean value specifying the publishing state of the content type.</span></span>

## <a name="request-body"></a><span data-ttu-id="0f483-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0f483-127">Request body</span></span>
<span data-ttu-id="0f483-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0f483-128">Do not supply a request body for this method.</span></span>

## <a name="example"></a><span data-ttu-id="0f483-129">Пример</span><span class="sxs-lookup"><span data-stu-id="0f483-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f483-130">Запрос</span><span class="sxs-lookup"><span data-stu-id="0f483-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "contenttype_ispublished"
}
-->
```http
GET https://graph.microsoft.com/beta/sites/{siteId}/contentTypes/{contentTypeId}/isPublished
```
### <a name="response"></a><span data-ttu-id="0f483-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0f483-131">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string"
}
-->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": true 
}
```

[contentType]: ../resources/contentType.md
