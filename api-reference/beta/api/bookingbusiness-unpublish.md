---
title: 'bookingBusiness: Отмена публикации'
description: Доступность планирования страницы бизнеса не для внешних клиентов.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 0b6c8122d37e5f6cdb1698b0d86295156e3481a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517528"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="00bf8-103">bookingBusiness: Отмена публикации</span><span class="sxs-lookup"><span data-stu-id="00bf8-103">bookingBusiness: unpublish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="00bf8-104">Доступность планирования страницы бизнеса не для внешних клиентов.</span><span class="sxs-lookup"><span data-stu-id="00bf8-104">Make the scheduling page of this business not available to external customers.</span></span>

<span data-ttu-id="00bf8-105">Присвойте свойству **isPublished** значение false и свойство **publicUrl** значения NULL.</span><span class="sxs-lookup"><span data-stu-id="00bf8-105">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="00bf8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="00bf8-106">Permissions</span></span>
<span data-ttu-id="00bf8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="00bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00bf8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="00bf8-109">Permission type</span></span>      | <span data-ttu-id="00bf8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="00bf8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00bf8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="00bf8-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="00bf8-112">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="00bf8-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="00bf8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="00bf8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="00bf8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00bf8-114">Not supported.</span></span>   |
|<span data-ttu-id="00bf8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="00bf8-115">Application</span></span> | <span data-ttu-id="00bf8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00bf8-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="00bf8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="00bf8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="00bf8-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="00bf8-118">Request headers</span></span>
| <span data-ttu-id="00bf8-119">Имя</span><span class="sxs-lookup"><span data-stu-id="00bf8-119">Name</span></span>       | <span data-ttu-id="00bf8-120">Описание</span><span class="sxs-lookup"><span data-stu-id="00bf8-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="00bf8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="00bf8-121">Authorization</span></span>  | <span data-ttu-id="00bf8-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="00bf8-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="00bf8-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="00bf8-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="00bf8-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="00bf8-124">Response</span></span>
<span data-ttu-id="00bf8-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="00bf8-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00bf8-127">Пример</span><span class="sxs-lookup"><span data-stu-id="00bf8-127">Example</span></span>
<span data-ttu-id="00bf8-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="00bf8-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="00bf8-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="00bf8-129">Request</span></span>
<span data-ttu-id="00bf8-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="00bf8-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="00bf8-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="00bf8-131">Response</span></span>
<span data-ttu-id="00bf8-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="00bf8-132">The following is an example of the response.</span></span>
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
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingbusiness-unpublish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
