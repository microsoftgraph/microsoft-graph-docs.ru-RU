---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8e59a7aea74e165945757f2513102a66baf64be1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27920242"
---
# <a name="sitepage-publish"></a><span data-ttu-id="891ad-102">sitePage: публикация</span><span class="sxs-lookup"><span data-stu-id="891ad-102">sitePage: publish</span></span>

> <span data-ttu-id="891ad-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="891ad-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="891ad-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="891ad-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="891ad-105">Публикация последней версии ресурсов [sitePage][] , предоставляющего версии страницы для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="891ad-105">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="891ad-106">Если страница извлечена, вернуть ее и опубликовать его.</span><span class="sxs-lookup"><span data-stu-id="891ad-106">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="891ad-107">Если страница извлечена вызывающему этот интерфейс API, страница автоматически вернули и последующей публикацией.</span><span class="sxs-lookup"><span data-stu-id="891ad-107">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="891ad-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="891ad-109">Permissions</span></span>

<span data-ttu-id="891ad-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="891ad-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="891ad-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="891ad-112">Permission type</span></span>      | <span data-ttu-id="891ad-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="891ad-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="891ad-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="891ad-114">Delegated (work or school account)</span></span> | <span data-ttu-id="891ad-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891ad-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="891ad-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="891ad-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="891ad-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891ad-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="891ad-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="891ad-118">Application</span></span> | <span data-ttu-id="891ad-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="891ad-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="891ad-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="891ad-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="891ad-121">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="891ad-121">Request body</span></span>

<span data-ttu-id="891ad-122">Это сообщение не имеет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="891ad-122">This message does not have a request body.</span></span> <span data-ttu-id="891ad-123">Любой текст запроса отправляются будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="891ad-123">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="891ad-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="891ad-124">Response</span></span>

<span data-ttu-id="891ad-125">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="891ad-125">If successful, the API call returns a `204 No Content`.</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
