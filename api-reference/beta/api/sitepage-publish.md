---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Страница публикации
ms.openlocfilehash: d932b1d37b5ab81f86f6e87aab43aa1cf9dc3eae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076402"
---
# <a name="sitepage-publish"></a><span data-ttu-id="d1910-102">sitePage: публикация</span><span class="sxs-lookup"><span data-stu-id="d1910-102">sitePage: publish</span></span>

> <span data-ttu-id="d1910-103">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1910-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1910-104">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1910-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1910-105">Публикация последней версии ресурсов [sitePage][] , предоставляющего версии страницы для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="d1910-105">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="d1910-106">Если страница извлечена, вернуть ее и опубликовать его.</span><span class="sxs-lookup"><span data-stu-id="d1910-106">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="d1910-107">Если страница извлечена вызывающему этот интерфейс API, страница автоматически вернули и последующей публикацией.</span><span class="sxs-lookup"><span data-stu-id="d1910-107">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="d1910-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d1910-109">Permissions</span></span>

<span data-ttu-id="d1910-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d1910-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d1910-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d1910-112">Permission type</span></span>      | <span data-ttu-id="d1910-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d1910-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1910-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d1910-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d1910-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1910-115">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1910-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d1910-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1910-117">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1910-117">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="d1910-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d1910-118">Application</span></span> | <span data-ttu-id="d1910-119">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d1910-119">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1910-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d1910-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="d1910-121">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d1910-121">Request body</span></span>

<span data-ttu-id="d1910-122">Это сообщение не имеет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="d1910-122">This message does not have a request body.</span></span> <span data-ttu-id="d1910-123">Любой текст запроса отправляются будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="d1910-123">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="d1910-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="d1910-124">Response</span></span>

<span data-ttu-id="d1910-125">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d1910-125">If successful, the API call returns a `204 No Content`.</span></span>

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
