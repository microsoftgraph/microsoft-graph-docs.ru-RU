---
title: Получение объекта unfamiliarLocationRiskEvent
description: Получение свойств и связей объекта унфамилиарлокатионрискевент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 727bb16d43589019ce5272e3e9e8c6e04499ce44
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178935"
---
# <a name="get-unfamiliarlocationriskevent"></a><span data-ttu-id="47bfb-103">Получение объекта unfamiliarLocationRiskEvent</span><span class="sxs-lookup"><span data-stu-id="47bfb-103">Get unfamiliarLocationRiskEvent</span></span>

<span data-ttu-id="47bfb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47bfb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="47bfb-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="47bfb-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="47bfb-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="47bfb-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="47bfb-107">Получение свойств и связей объекта унфамилиарлокатионрискевент.</span><span class="sxs-lookup"><span data-stu-id="47bfb-107">Retrieve the properties and relationships of an unfamiliarlocationriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="47bfb-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="47bfb-108">Permissions</span></span>
<span data-ttu-id="47bfb-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47bfb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47bfb-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="47bfb-111">Permission type</span></span>      | <span data-ttu-id="47bfb-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="47bfb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="47bfb-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="47bfb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="47bfb-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="47bfb-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="47bfb-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="47bfb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="47bfb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="47bfb-116">Not supported.</span></span>    |
|<span data-ttu-id="47bfb-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="47bfb-117">Application</span></span> | <span data-ttu-id="47bfb-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="47bfb-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="47bfb-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="47bfb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /unfamiliarLocationRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="47bfb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="47bfb-120">Request headers</span></span>
| <span data-ttu-id="47bfb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="47bfb-121">Name</span></span>      |<span data-ttu-id="47bfb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="47bfb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="47bfb-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="47bfb-123">Authorization</span></span>  | <span data-ttu-id="47bfb-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="47bfb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="47bfb-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="47bfb-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="47bfb-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="47bfb-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="47bfb-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="47bfb-129">Request body</span></span>
<span data-ttu-id="47bfb-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="47bfb-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="47bfb-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="47bfb-131">Response</span></span>

<span data-ttu-id="47bfb-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [унфамилиарлокатионрискевент](../resources/unfamiliarlocationriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="47bfb-132">If successful, this method returns a `200 OK` response code and [unfamiliarLocationRiskEvent](../resources/unfamiliarlocationriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="47bfb-133">Пример</span><span class="sxs-lookup"><span data-stu-id="47bfb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="47bfb-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="47bfb-134">Request</span></span>
<span data-ttu-id="47bfb-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="47bfb-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_unfamiliarlocationriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/unfamiliarLocationRiskEvents/700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604
```
##### <a name="response"></a><span data-ttu-id="47bfb-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="47bfb-136">Response</span></span>
<span data-ttu-id="47bfb-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="47bfb-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unfamiliarLocationRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "closedDateTime": "2016-01-29T20:03:57.7872426Z",
  "createdDateTime": "2016-01-29T00:01:49.126468Z",
  "id": "700b6476-8138-4c14-4962-c43614958301-8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad-4e5591fd-2ac1-4e9d-96a9-aca8339e2604",
  "ipAddress": "176.10.104.240",
  "location": "Bern, CH",
  "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
  "riskEventStatus": "remediated",
  "riskLevel": "medium",
  "riskType": "UnfamiliarLocationRiskEvent",
  "userDisplayName": "Jon Doe",
  "userId": "8dce9c6b-21f1-2e3b-2c3b-5164f751e7ad",
  "userPrincipalName": "jon@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get unfamiliarLocationRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
