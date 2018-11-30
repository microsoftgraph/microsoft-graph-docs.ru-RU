---
title: 'bookingBusiness: публикация'
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: b3145409de1371a164d86ad1cc52ea199d245f50
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076683"
---
# <a name="bookingbusiness-publish"></a><span data-ttu-id="64503-104">bookingBusiness: публикация</span><span class="sxs-lookup"><span data-stu-id="64503-104">bookingBusiness: publish</span></span>

 > <span data-ttu-id="64503-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="64503-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="64503-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64503-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="64503-107">Сделайте доступными странице планирования бизнеса внешним клиентам.</span><span class="sxs-lookup"><span data-stu-id="64503-107">Make the scheduling page of this business available to external customers.</span></span> 

<span data-ttu-id="64503-108">Свойства **isPublished** значение true, а свойство **publicUrl** URL-адрес страницы планирования.</span><span class="sxs-lookup"><span data-stu-id="64503-108">Set the **isPublished** property to true, and **publicUrl** property to the URL of the scheduling page.</span></span>

## <a name="permissions"></a><span data-ttu-id="64503-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="64503-109">Permissions</span></span>
<span data-ttu-id="64503-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="64503-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="64503-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="64503-112">Permission type</span></span>      | <span data-ttu-id="64503-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="64503-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64503-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="64503-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="64503-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="64503-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="64503-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="64503-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64503-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64503-117">Not supported.</span></span>   |
|<span data-ttu-id="64503-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="64503-118">Application</span></span> | <span data-ttu-id="64503-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="64503-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="64503-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="64503-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/publish

```
## <a name="request-headers"></a><span data-ttu-id="64503-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="64503-121">Request headers</span></span>
| <span data-ttu-id="64503-122">Имя</span><span class="sxs-lookup"><span data-stu-id="64503-122">Name</span></span>       | <span data-ttu-id="64503-123">Описание</span><span class="sxs-lookup"><span data-stu-id="64503-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64503-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="64503-124">Authorization</span></span>  | <span data-ttu-id="64503-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="64503-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="64503-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="64503-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="64503-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="64503-127">Response</span></span>
<span data-ttu-id="64503-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="64503-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64503-130">Пример</span><span class="sxs-lookup"><span data-stu-id="64503-130">Example</span></span>
<span data-ttu-id="64503-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="64503-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="64503-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="64503-132">Request</span></span>
<span data-ttu-id="64503-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="64503-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_publish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/publish
```

##### <a name="response"></a><span data-ttu-id="64503-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="64503-134">Response</span></span>
<span data-ttu-id="64503-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="64503-135">The following is an example of the response.</span></span> 
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
<!-- {
  "type": "#page.annotation",
  "description": "bookingBusiness: publish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->