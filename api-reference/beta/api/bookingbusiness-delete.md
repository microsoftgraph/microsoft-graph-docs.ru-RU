---
title: Удаление bookingBusiness
description: " > **Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается."
ms.openlocfilehash: d920414bb73f506c4e94cb973642c124544fc1bf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076328"
---
# <a name="delete-bookingbusiness"></a><span data-ttu-id="10e09-104">Удаление bookingBusiness</span><span class="sxs-lookup"><span data-stu-id="10e09-104">Delete bookingBusiness</span></span>

 > <span data-ttu-id="10e09-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="10e09-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10e09-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10e09-106">Use of these APIs in production applications is not supported.</span></span>
 
<span data-ttu-id="10e09-107">Удалите объект [bookingBusiness](../resources/bookingbusiness.md) .</span><span class="sxs-lookup"><span data-stu-id="10e09-107">Delete a [bookingBusiness](../resources/bookingbusiness.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="10e09-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="10e09-108">Permissions</span></span>
<span data-ttu-id="10e09-p103">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="10e09-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10e09-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="10e09-111">Permission type</span></span>      | <span data-ttu-id="10e09-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="10e09-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="10e09-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="10e09-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="10e09-114">Bookings.Manage.All</span><span class="sxs-lookup"><span data-stu-id="10e09-114">Bookings.Manage.All</span></span>   |
|<span data-ttu-id="10e09-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="10e09-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="10e09-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10e09-116">Not supported.</span></span>   |
|<span data-ttu-id="10e09-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="10e09-117">Application</span></span> | <span data-ttu-id="10e09-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="10e09-118">Not supported.</span></span>  | 

## <a name="http-request"></a><span data-ttu-id="10e09-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="10e09-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/<id>

```
## <a name="request-headers"></a><span data-ttu-id="10e09-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="10e09-120">Request headers</span></span>
| <span data-ttu-id="10e09-121">Имя</span><span class="sxs-lookup"><span data-stu-id="10e09-121">Name</span></span>       | <span data-ttu-id="10e09-122">Описание</span><span class="sxs-lookup"><span data-stu-id="10e09-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="10e09-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10e09-123">Authorization</span></span>  | <span data-ttu-id="10e09-124">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="10e09-124">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="10e09-125">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="10e09-125">Request body</span></span>
<span data-ttu-id="10e09-126">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="10e09-126">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="10e09-127">Отклик</span><span class="sxs-lookup"><span data-stu-id="10e09-127">Response</span></span>
<span data-ttu-id="10e09-p104">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="10e09-p104">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10e09-130">Пример</span><span class="sxs-lookup"><span data-stu-id="10e09-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="10e09-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="10e09-131">Request</span></span>
<span data-ttu-id="10e09-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="10e09-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingbusiness"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/fabrikam@M365B489948.onmicrosoft.com
```
##### <a name="response"></a><span data-ttu-id="10e09-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="10e09-133">Response</span></span>
<span data-ttu-id="10e09-134">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="10e09-134">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete bookingBusiness",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->