---
title: Удаление Букингкустомер
description: Удаление указанного объекта Букингкустомер.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: 767dea301d554e2ec0131d373b2206b0ef87db6a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461833"
---
# <a name="delete-bookingcustomer"></a><span data-ttu-id="cd2af-103">Удаление Букингкустомер</span><span class="sxs-lookup"><span data-stu-id="cd2af-103">Delete bookingCustomer</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cd2af-104">Удаление указанного объекта [букингкустомер](../resources/bookingcustomer.md) .</span><span class="sxs-lookup"><span data-stu-id="cd2af-104">Delete the specified [bookingCustomer](../resources/bookingcustomer.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="cd2af-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="cd2af-105">Permissions</span></span>
<span data-ttu-id="cd2af-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd2af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd2af-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="cd2af-108">Permission type</span></span>      | <span data-ttu-id="cd2af-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="cd2af-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd2af-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="cd2af-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cd2af-111">Букингсаппоинтмент. ReadWrite. ALL, Books. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="cd2af-111">BookingsAppointment.ReadWrite.All, Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="cd2af-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="cd2af-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd2af-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd2af-113">Not supported.</span></span>   |
|<span data-ttu-id="cd2af-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="cd2af-114">Application</span></span> | <span data-ttu-id="cd2af-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cd2af-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cd2af-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="cd2af-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/customers/{id}

```
## <a name="request-headers"></a><span data-ttu-id="cd2af-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="cd2af-117">Request headers</span></span>
| <span data-ttu-id="cd2af-118">Имя</span><span class="sxs-lookup"><span data-stu-id="cd2af-118">Name</span></span>       | <span data-ttu-id="cd2af-119">Описание</span><span class="sxs-lookup"><span data-stu-id="cd2af-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cd2af-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="cd2af-120">Authorization</span></span>  | <span data-ttu-id="cd2af-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="cd2af-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd2af-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="cd2af-122">Request body</span></span>
<span data-ttu-id="cd2af-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="cd2af-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="cd2af-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd2af-124">Response</span></span>
<span data-ttu-id="cd2af-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="cd2af-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd2af-127">Пример</span><span class="sxs-lookup"><span data-stu-id="cd2af-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cd2af-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="cd2af-128">Request</span></span>
<span data-ttu-id="cd2af-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="cd2af-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingcustomer"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/customers/80b5ddda-1e3b-4c9d-abe2-d606cc075e2e
```
##### <a name="response"></a><span data-ttu-id="cd2af-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="cd2af-130">Response</span></span>
<span data-ttu-id="cd2af-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="cd2af-131">The following is an example of the response.</span></span> <span data-ttu-id="cd2af-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="cd2af-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="cd2af-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="cd2af-133">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete bookingCustomer",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingcustomer-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
