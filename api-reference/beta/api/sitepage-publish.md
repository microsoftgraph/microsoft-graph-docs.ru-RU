---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: d9bf699c0038e785a11560ee7326cfb2324345f3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335899"
---
# <a name="sitepage-publish"></a><span data-ttu-id="b4683-102">Ситепаже: публикация</span><span class="sxs-lookup"><span data-stu-id="b4683-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4683-103">Опубликуйте последнюю версию ресурса [ситепаже][] , которая делает версию страницы доступной для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="b4683-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="b4683-104">Если страница извлечена, необходимо вернуть страницу и опубликовать ее.</span><span class="sxs-lookup"><span data-stu-id="b4683-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="b4683-105">Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.</span><span class="sxs-lookup"><span data-stu-id="b4683-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="b4683-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b4683-107">Permissions</span></span>

<span data-ttu-id="b4683-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b4683-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4683-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b4683-110">Permission type</span></span>      | <span data-ttu-id="b4683-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b4683-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4683-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b4683-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b4683-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4683-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4683-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b4683-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b4683-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4683-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b4683-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b4683-116">Application</span></span> | <span data-ttu-id="b4683-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b4683-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b4683-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b4683-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="b4683-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b4683-119">Request body</span></span>

<span data-ttu-id="b4683-120">У этого сообщения нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="b4683-120">This message does not have a request body.</span></span> <span data-ttu-id="b4683-121">Любой Отправленный текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="b4683-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="b4683-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="b4683-122">Response</span></span>

<span data-ttu-id="b4683-123">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b4683-123">If successful, the API call returns a `204 No Content`.</span></span>

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
