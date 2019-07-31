---
author: rahmit
description: Опубликуйте последнюю версию ресурса Ситепаже, которая делает версию страницы доступной для всех пользователей. Если страница извлечена, необходимо вернуть страницу и опубликовать ее. Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5f4404b33a54979271750d4074a9c6da235966ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991214"
---
# <a name="sitepage-publish"></a><span data-ttu-id="e92de-105">Ситепаже: публикация</span><span class="sxs-lookup"><span data-stu-id="e92de-105">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e92de-106">Опубликуйте последнюю версию ресурса [ситепаже][] , которая делает версию страницы доступной для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="e92de-106">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="e92de-107">Если страница извлечена, необходимо вернуть страницу и опубликовать ее.</span><span class="sxs-lookup"><span data-stu-id="e92de-107">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="e92de-108">Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.</span><span class="sxs-lookup"><span data-stu-id="e92de-108">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="e92de-110">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e92de-110">Permissions</span></span>

<span data-ttu-id="e92de-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e92de-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e92de-113">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e92de-113">Permission type</span></span>      | <span data-ttu-id="e92de-114">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e92de-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e92de-115">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e92de-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e92de-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e92de-116">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e92de-117">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e92de-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e92de-118">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e92de-118">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e92de-119">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e92de-119">Application</span></span> | <span data-ttu-id="e92de-120">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e92de-120">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e92de-121">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e92de-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="e92de-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="e92de-122">Request body</span></span>

<span data-ttu-id="e92de-123">У этого сообщения нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="e92de-123">This message does not have a request body.</span></span> <span data-ttu-id="e92de-124">Любой Отправленный текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="e92de-124">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="e92de-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="e92de-125">Response</span></span>

<span data-ttu-id="e92de-126">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e92de-126">If successful, the API call returns a `204 No Content`.</span></span>

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
