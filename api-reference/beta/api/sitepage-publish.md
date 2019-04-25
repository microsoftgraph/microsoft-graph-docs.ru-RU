---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Страница публикации
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545241"
---
# <a name="sitepage-publish"></a><span data-ttu-id="def25-102">Ситепаже: публикация</span><span class="sxs-lookup"><span data-stu-id="def25-102">sitePage: publish</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="def25-103">Опубликуйте последнюю версию ресурса [ситепаже][] , которая делает версию страницы доступной для всех пользователей.</span><span class="sxs-lookup"><span data-stu-id="def25-103">Publish the latest version of a [sitePage][] resource, which makes the version of the page available to all users.</span></span> <span data-ttu-id="def25-104">Если страница извлечена, необходимо вернуть страницу и опубликовать ее.</span><span class="sxs-lookup"><span data-stu-id="def25-104">If the page is checked out, check in the page and publish it.</span></span> <span data-ttu-id="def25-105">Если страница извлечена в вызывающий объект этого API, страница автоматически возвращается и затем публикуется.</span><span class="sxs-lookup"><span data-stu-id="def25-105">If the page is checked out to the caller of this API, the page is automatically checked in and then published.</span></span>

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a><span data-ttu-id="def25-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="def25-107">Permissions</span></span>

<span data-ttu-id="def25-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="def25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="def25-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="def25-110">Permission type</span></span>      | <span data-ttu-id="def25-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="def25-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="def25-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="def25-112">Delegated (work or school account)</span></span> | <span data-ttu-id="def25-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def25-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="def25-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="def25-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="def25-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def25-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="def25-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="def25-116">Application</span></span> | <span data-ttu-id="def25-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="def25-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="def25-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="def25-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a><span data-ttu-id="def25-119">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="def25-119">Request body</span></span>

<span data-ttu-id="def25-120">У этого сообщения нет текста запроса.</span><span class="sxs-lookup"><span data-stu-id="def25-120">This message does not have a request body.</span></span> <span data-ttu-id="def25-121">Любой Отправленный текст запроса будет игнорироваться.</span><span class="sxs-lookup"><span data-stu-id="def25-121">Any request body sent will be ignored.</span></span>

## <a name="response"></a><span data-ttu-id="def25-122">Отклик</span><span class="sxs-lookup"><span data-stu-id="def25-122">Response</span></span>

<span data-ttu-id="def25-123">При успешном выполнении вызова API возвращается отклик `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="def25-123">If successful, the API call returns a `204 No Content`.</span></span>

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
