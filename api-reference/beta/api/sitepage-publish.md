---
author: rahmit
description: Опубликуйте последнюю версию ресурса Ситепаже, которая делает версию страницы доступной для всех пользователей. Если страница извлечена, необходимо вернуть страницу и опубликовать ее. Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 90d08b3f8fae2ed186d1809b4318eec7ef9cf5dc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453172"
---
# <a name="sitepage-publish"></a><span data-ttu-id="bc7a0-105">Ситепаже: публикация</span><span class="sxs-lookup"><span data-stu-id="bc7a0-105">sitePage: publish</span></span>

<span data-ttu-id="bc7a0-106">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bc7a0-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc7a0-107">Опубликуйте последнюю версию ресурса [ситепаже][] , которая делает версию страницы доступной для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="bc7a0-107">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="bc7a0-108">Если страница извлечена, необходимо вернуть страницу и опубликовать ее.</span><span class="sxs-lookup"><span data-stu-id="bc7a0-108">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="bc7a0-109">Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.</span><span class="sxs-lookup"><span data-stu-id="bc7a0-109">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="bc7a0-111">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bc7a0-111">Permissions</span></span>

<span data-ttu-id="bc7a0-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bc7a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bc7a0-114">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bc7a0-114">Permission type</span></span>      | <span data-ttu-id="bc7a0-115">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="bc7a0-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc7a0-116">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bc7a0-116">Delegated (work or school account)</span></span> | <span data-ttu-id="bc7a0-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7a0-117">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc7a0-118">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bc7a0-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc7a0-119">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7a0-119">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="bc7a0-120">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bc7a0-120">Application</span></span> | <span data-ttu-id="bc7a0-121">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bc7a0-121">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc7a0-122">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bc7a0-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="bc7a0-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bc7a0-123">Request body</span></span>

<span data-ttu-id="bc7a0-124">У этого сообщения нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="bc7a0-124">This message does not have a request body.</span></span> <span data-ttu-id="bc7a0-125">Любой Отправленный текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="bc7a0-125">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="bc7a0-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="bc7a0-126">Response</span></span>

<span data-ttu-id="bc7a0-127">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="bc7a0-127">If successful, the API call returns a `204 No Content`.</span></span>

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
