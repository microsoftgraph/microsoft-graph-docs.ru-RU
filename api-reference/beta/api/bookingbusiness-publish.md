---
title: 'Букингбусинесс: публикация'
description: Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: d6fae2c6d39f3abe2b460fe71863c7b570fa340b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322546"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="0ae16-103">Букингбусинесс: публикация</span><span class="sxs-lookup"><span data-stu-id="0ae16-103">bookingBusiness: publish</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ae16-104">Сделайте страницу планирования для этого бизнеса доступной внешним клиентам.</span><span class="sxs-lookup"><span data-stu-id="0ae16-104">Make the scheduling page of this business available to external customers.</span></span>

<span data-ttu-id="0ae16-105">Задайте для свойства **публикации** значение true, а свойству **ПУБЛИКУРЛ** — URL-адрес страницы планирования.</span><span class="sxs-lookup"><span data-stu-id="0ae16-105">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ae16-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0ae16-106">Permissions</span></span>
<span data-ttu-id="0ae16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ae16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ae16-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0ae16-109">Permission type</span></span>      | <span data-ttu-id="0ae16-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0ae16-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ae16-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0ae16-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="0ae16-112">Резервирования. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="0ae16-112">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="0ae16-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0ae16-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ae16-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae16-114">Not supported.</span></span>   |
|<span data-ttu-id="0ae16-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0ae16-115">Application</span></span> | <span data-ttu-id="0ae16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ae16-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0ae16-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0ae16-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="0ae16-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0ae16-118">Request headers</span></span>
| <span data-ttu-id="0ae16-119">Имя</span><span class="sxs-lookup"><span data-stu-id="0ae16-119">Name</span></span>       | <span data-ttu-id="0ae16-120">Описание</span><span class="sxs-lookup"><span data-stu-id="0ae16-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ae16-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0ae16-121">Authorization</span></span>  | <span data-ttu-id="0ae16-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="0ae16-122">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ae16-123">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0ae16-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="0ae16-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ae16-124">Response</span></span>
<span data-ttu-id="0ae16-p102">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="0ae16-p102">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ae16-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0ae16-127">Example</span></span>
<span data-ttu-id="0ae16-128">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="0ae16-128">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0ae16-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="0ae16-129">Request</span></span>
<span data-ttu-id="0ae16-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0ae16-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="0ae16-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="0ae16-131">Response</span></span>
<span data-ttu-id="0ae16-132">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="0ae16-132">The following is an example of the response.</span></span>
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
  "suppressions": []
}
-->
