---
title: 'Букингбусинесс: публикация'
description: Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 11d8bea864772c0bcc4365c056973fac782add5d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462013"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="a289c-103">Букингбусинесс: публикация</span><span class="sxs-lookup"><span data-stu-id="a289c-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a289c-104">Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.</span><span class="sxs-lookup"><span data-stu-id="a289c-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="a289c-105">Задайте для свойства **публикации** значение true, а свойству **ПУБЛИКУРЛ** — URL-адрес страницы планирования.</span><span class="sxs-lookup"><span data-stu-id="a289c-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="a289c-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a289c-106">Permissions</span></span>
<span data-ttu-id="a289c-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a289c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a289c-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a289c-109">Permission type</span></span>      | <span data-ttu-id="a289c-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a289c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a289c-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a289c-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="a289c-112">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="a289c-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="a289c-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a289c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a289c-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a289c-114">Not supported.</span></span>   |
|<span data-ttu-id="a289c-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a289c-115">Application</span></span> | <span data-ttu-id="a289c-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a289c-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="a289c-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a289c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="a289c-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a289c-118">Request headers</span></span>
| <span data-ttu-id="a289c-119">Имя</span><span class="sxs-lookup"><span data-stu-id="a289c-119">Name</span></span>       | <span data-ttu-id="a289c-120">Описание</span><span class="sxs-lookup"><span data-stu-id="a289c-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a289c-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a289c-121">Authorization</span></span>  | <span data-ttu-id="a289c-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="a289c-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="a289c-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a289c-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="a289c-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="a289c-124">Response</span></span>
<span data-ttu-id="a289c-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="a289c-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a289c-127">Пример</span><span class="sxs-lookup"><span data-stu-id="a289c-127">Example</span></span>
<span data-ttu-id="a289c-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="a289c-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a289c-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="a289c-129">Request</span></span>
<span data-ttu-id="a289c-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="a289c-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="a289c-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="a289c-131">Response</span></span>
<span data-ttu-id="a289c-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="a289c-132">The following is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
