---
author: rahmit
description: Опубликуйте последнюю версию ресурса Ситепаже, которая делает версию страницы доступной для всех пользователей. Если страница извлечена, необходимо вернуть страницу и опубликовать ее. Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e40f864ce224916a2c60e5c82e0aecbfff213fbc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044384"
---
# <a name="sitepage-publish"></a><span data-ttu-id="c197d-105">Ситепаже: публикация</span><span class="sxs-lookup"><span data-stu-id="c197d-105">sitePage: publish</span></span>

<span data-ttu-id="c197d-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c197d-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c197d-107">Опубликуйте последнюю версию ресурса [ситепаже][] , которая делает версию страницы доступной для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="c197d-107">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="c197d-108">Если страница извлечена, необходимо вернуть страницу и опубликовать ее.</span><span class="sxs-lookup"><span data-stu-id="c197d-108">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="c197d-109">Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.</span><span class="sxs-lookup"><span data-stu-id="c197d-109">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="c197d-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c197d-111">Permissions</span></span>

<span data-ttu-id="c197d-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c197d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c197d-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c197d-114">Permission type</span></span>      | <span data-ttu-id="c197d-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c197d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c197d-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c197d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="c197d-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c197d-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c197d-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c197d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c197d-119">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c197d-119">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c197d-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c197d-120">Application</span></span> | <span data-ttu-id="c197d-121">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c197d-121">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c197d-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c197d-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="c197d-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c197d-123">Request body</span></span>

<span data-ttu-id="c197d-124">У этого сообщения нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="c197d-124">This message does not have a request body.</span></span> <span data-ttu-id="c197d-125">Любой Отправленный текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="c197d-125">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="c197d-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="c197d-126">Response</span></span>

<span data-ttu-id="c197d-127">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="c197d-127">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": []
}
-->


