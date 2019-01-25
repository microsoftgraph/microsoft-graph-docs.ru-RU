---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507532"
---
# <a name="sitepage-publish"></a><span data-ttu-id="1814b-102">sitePage: публикация</span><span class="sxs-lookup"><span data-stu-id="1814b-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1814b-103">Публикация последней версии ресурсов [sitePage][] , предоставляющего версии страницы для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="1814b-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="1814b-104">Если страница извлечена, вернуть ее и опубликовать его.</span><span class="sxs-lookup"><span data-stu-id="1814b-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="1814b-105">Если страница извлечена вызывающему этот интерфейс API, страница автоматически вернули и последующей публикацией.</span><span class="sxs-lookup"><span data-stu-id="1814b-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="1814b-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1814b-107">Permissions</span></span>

<span data-ttu-id="1814b-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1814b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1814b-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1814b-110">Permission type</span></span>      | <span data-ttu-id="1814b-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1814b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1814b-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1814b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1814b-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1814b-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1814b-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1814b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1814b-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1814b-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1814b-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1814b-116">Application</span></span> | <span data-ttu-id="1814b-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1814b-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1814b-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1814b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="1814b-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1814b-119">Request body</span></span>

<span data-ttu-id="1814b-120">Это сообщение не имеет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="1814b-120">This message does not have a request body.</span></span> <span data-ttu-id="1814b-121">Любой текст запроса отправляются будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="1814b-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="1814b-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="1814b-122">Response</span></span>

<span data-ttu-id="1814b-123">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="1814b-123">If successful, the API call returns a `204 No Content`.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
