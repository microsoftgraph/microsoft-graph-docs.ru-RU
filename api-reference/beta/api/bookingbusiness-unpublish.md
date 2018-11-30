---
title: 'bookingBusiness: Отмена публикации'
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: 7d0e083eded3ce0c1328c9532358cf7a054db52b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27077004"
---
# <a name="bookingbusiness-unpublish"></a><span data-ttu-id="ff2a9-104">bookingBusiness: Отмена публикации</span><span class="sxs-lookup"><span data-stu-id="ff2a9-104">bookingBusiness: unpublish</span></span>

 > <span data-ttu-id="ff2a9-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff2a9-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="ff2a9-107">Доступность планирования страницы бизнеса не для внешних клиентов.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-107">Make the scheduling page of this business not available to external customers.</span></span> 

<span data-ttu-id="ff2a9-108">Присвойте свойству **isPublished** значение false и свойство **publicUrl** значения NULL.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-108">Set the **isPublished** property to false, and **publicUrl** property to null.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff2a9-109">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ff2a9-109">Permissions</span></span>
<span data-ttu-id="ff2a9-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ff2a9-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff2a9-112">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ff2a9-112">Permission type</span></span>      | <span data-ttu-id="ff2a9-113">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ff2a9-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff2a9-114">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ff2a9-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="ff2a9-115">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="ff2a9-115">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="ff2a9-116">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ff2a9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff2a9-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-117">Not supported.</span></span>   |
|<span data-ttu-id="ff2a9-118">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ff2a9-118">Application</span></span> | <span data-ttu-id="ff2a9-119">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-119">Not supported.</span></span>  |  

## <a name="http-request"></a><span data-ttu-id="ff2a9-120">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ff2a9-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /bookingBusinesses/{id}/unpublish

```
## <a name="request-headers"></a><span data-ttu-id="ff2a9-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ff2a9-121">Request headers</span></span>
| <span data-ttu-id="ff2a9-122">Имя</span><span class="sxs-lookup"><span data-stu-id="ff2a9-122">Name</span></span>       | <span data-ttu-id="ff2a9-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ff2a9-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ff2a9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff2a9-124">Authorization</span></span>  | <span data-ttu-id="ff2a9-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="ff2a9-125">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff2a9-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="ff2a9-126">Request body</span></span>

## <a name="response"></a><span data-ttu-id="ff2a9-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="ff2a9-127">Response</span></span>
<span data-ttu-id="ff2a9-p104">В случае успешного выполнения этот метод возвращает код отклика `204 No content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-p104">If successful, this method returns `204 No content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff2a9-130">Пример</span><span class="sxs-lookup"><span data-stu-id="ff2a9-130">Example</span></span>
<span data-ttu-id="ff2a9-131">Ниже приведен пример вызова этого API.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-131">The following is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="ff2a9-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="ff2a9-132">Request</span></span>
<span data-ttu-id="ff2a9-133">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "bookingbusiness_unpublish"
}-->
```http
POST https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/unpublish
```

##### <a name="response"></a><span data-ttu-id="ff2a9-134">Ответ</span><span class="sxs-lookup"><span data-stu-id="ff2a9-134">Response</span></span>
<span data-ttu-id="ff2a9-135">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="ff2a9-135">The following is an example of the response.</span></span> 
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
  "description": "bookingBusiness: unpublish",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->