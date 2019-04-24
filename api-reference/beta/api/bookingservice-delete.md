---
title: Удаление Букингсервице
description: Удаление объекта Букингсервице в указанном букингбусинесс.
localization_priority: Normal
author: angelgolfer-ms
ms.prod: bookings
ms.openlocfilehash: a541796fbfa500cc6d99205598042818b4aa47ad
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461670"
---
# <a name="delete-bookingservice"></a><span data-ttu-id="b7dac-103">Удаление Букингсервице</span><span class="sxs-lookup"><span data-stu-id="b7dac-103">Delete bookingService</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7dac-104">Удаление объекта [букингсервице](../resources/bookingservice.md) в указанном [букингбусинесс](../resources/bookingbusiness.md).</span><span class="sxs-lookup"><span data-stu-id="b7dac-104">Delete a [bookingService](../resources/bookingservice.md) object in the specified [bookingbusiness](../resources/bookingbusiness.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="b7dac-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b7dac-105">Permissions</span></span>
<span data-ttu-id="b7dac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b7dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7dac-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b7dac-108">Permission type</span></span>      | <span data-ttu-id="b7dac-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b7dac-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b7dac-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b7dac-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="b7dac-111">Резервирования. ReadWrite. ALL, Books. Manage. ALL</span><span class="sxs-lookup"><span data-stu-id="b7dac-111">Bookings.ReadWrite.All, Bookings.Manage.All</span></span>   |
|<span data-ttu-id="b7dac-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b7dac-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b7dac-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7dac-113">Not supported.</span></span>   |
|<span data-ttu-id="b7dac-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b7dac-114">Application</span></span> | <span data-ttu-id="b7dac-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7dac-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="b7dac-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b7dac-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /bookingBusinesses/{id}/services/{id}

```
## <a name="request-headers"></a><span data-ttu-id="b7dac-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b7dac-117">Request headers</span></span>
| <span data-ttu-id="b7dac-118">Имя</span><span class="sxs-lookup"><span data-stu-id="b7dac-118">Name</span></span>       | <span data-ttu-id="b7dac-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b7dac-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b7dac-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b7dac-120">Authorization</span></span>  | <span data-ttu-id="b7dac-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b7dac-121">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7dac-122">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="b7dac-122">Request body</span></span>
<span data-ttu-id="b7dac-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="b7dac-123">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="b7dac-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7dac-124">Response</span></span>
<span data-ttu-id="b7dac-p102">В случае успешного выполнения этот метод возвращает код отклика `204, No Content`. В тексте отклика не возвращается никаких данных.</span><span class="sxs-lookup"><span data-stu-id="b7dac-p102">If successful, this method returns `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7dac-127">Пример</span><span class="sxs-lookup"><span data-stu-id="b7dac-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b7dac-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b7dac-128">Request</span></span>
<span data-ttu-id="b7dac-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b7dac-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_bookingservice"
}-->
```http
DELETE https://graph.microsoft.com/beta/bookingBusinesses/Contosolunchdelivery@M365B489948.onmicrosoft.com/services/57da6774-a087-4d69-b0e6-6fb82c339976
```
##### <a name="response"></a><span data-ttu-id="b7dac-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b7dac-130">Response</span></span>
<span data-ttu-id="b7dac-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="b7dac-131">The following is an example of the response.</span></span> <span data-ttu-id="b7dac-132">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="b7dac-132">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b7dac-133">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="b7dac-133">All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete bookingService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/bookingservice-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
