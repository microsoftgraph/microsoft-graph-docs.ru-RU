---
title: Список Анонимаусиприскевентс
description: Получение списка объектов анонимаусиприскевент.
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: cloudhandler
ms.openlocfilehash: 242d1ef696d83e1854a3de51130ec203b201182d
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43178977"
---
# <a name="list-anonymousipriskevents"></a><span data-ttu-id="39e54-103">Список Анонимаусиприскевентс</span><span class="sxs-lookup"><span data-stu-id="39e54-103">List anonymousIpRiskEvents</span></span>

<span data-ttu-id="39e54-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39e54-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="39e54-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="39e54-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="39e54-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="39e54-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="39e54-107">Получение списка объектов анонимаусиприскевент.</span><span class="sxs-lookup"><span data-stu-id="39e54-107">Retrieve a list of anonymousipriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="39e54-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="39e54-108">Permissions</span></span>
<span data-ttu-id="39e54-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="39e54-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="39e54-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="39e54-111">Permission type</span></span>      | <span data-ttu-id="39e54-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="39e54-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="39e54-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="39e54-113">Delegated (work or school account)</span></span> | <span data-ttu-id="39e54-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="39e54-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="39e54-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="39e54-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="39e54-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="39e54-116">Not supported.</span></span>    |
|<span data-ttu-id="39e54-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="39e54-117">Application</span></span> | <span data-ttu-id="39e54-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="39e54-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="39e54-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="39e54-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /anonymousIpRiskEvents
```

## <a name="request-headers"></a><span data-ttu-id="39e54-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="39e54-120">Request headers</span></span>
| <span data-ttu-id="39e54-121">Имя</span><span class="sxs-lookup"><span data-stu-id="39e54-121">Name</span></span>      |<span data-ttu-id="39e54-122">Описание</span><span class="sxs-lookup"><span data-stu-id="39e54-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="39e54-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="39e54-123">Authorization</span></span>  | <span data-ttu-id="39e54-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="39e54-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="39e54-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="39e54-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="39e54-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="39e54-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="39e54-129">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="39e54-129">Request body</span></span>
<span data-ttu-id="39e54-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="39e54-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="39e54-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="39e54-131">Response</span></span>

<span data-ttu-id="39e54-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [анонимаусиприскевент](../resources/anonymousipriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="39e54-132">If successful, this method returns a `200 OK` response code and collection of [anonymousIpRiskEvent](../resources/anonymousipriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="39e54-133">Пример</span><span class="sxs-lookup"><span data-stu-id="39e54-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="39e54-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="39e54-134">Request</span></span>
<span data-ttu-id="39e54-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="39e54-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_anonymousipriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/anonymousIpRiskEvents
```
##### <a name="response"></a><span data-ttu-id="39e54-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="39e54-136">Response</span></span>
<span data-ttu-id="39e54-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="39e54-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.anonymousIpRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 290

{
  "value": [
    {
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "2016-01-29T00:00:56.22556656a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
      "ipAddress": null,
      "location": null,
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "AnonymousIpRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "6a56d0b2-3c51-7c5e-bc1a-1ccdb3bd9c71",
      "userPrincipalName": "jon@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List anonymousIpRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
