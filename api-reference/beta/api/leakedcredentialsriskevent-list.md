---
title: Список Леакедкредентиалсрискевентс
description: Получение списка объектов леакедкредентиалсрискевент.
localization_priority: Normal
doc_type: apiPageType
author: cloudhandler
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 05d5ef51e702efcbc7f445c113691c69a951393e
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181233"
---
# <a name="list-leakedcredentialsriskevents"></a><span data-ttu-id="d288a-103">Список Леакедкредентиалсрискевентс</span><span class="sxs-lookup"><span data-stu-id="d288a-103">List leakedCredentialsRiskEvents</span></span>

<span data-ttu-id="d288a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d288a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
><span data-ttu-id="d288a-105">API **идентитирискевентс** устарел и не возвращает данные на 10 января 2020.</span><span class="sxs-lookup"><span data-stu-id="d288a-105">The **identityRiskEvents** API is deprecated and will stop returning data on January 10, 2020.</span></span> <span data-ttu-id="d288a-106">Дополнительные сведения см. [в разделе устаревшее API идентитирискевентс](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span><span class="sxs-lookup"><span data-stu-id="d288a-106">For details, see [Deprecation of the IdentityRiskEvents API](https://developer.microsoft.com/office/blogs/deprecatation-of-the-identityriskevents-api/).</span></span>

<span data-ttu-id="d288a-107">Получение списка объектов леакедкредентиалсрискевент.</span><span class="sxs-lookup"><span data-stu-id="d288a-107">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="d288a-108">Разрешения</span><span class="sxs-lookup"><span data-stu-id="d288a-108">Permissions</span></span>
<span data-ttu-id="d288a-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d288a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d288a-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="d288a-111">Permission type</span></span>      | <span data-ttu-id="d288a-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="d288a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d288a-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="d288a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="d288a-114">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="d288a-114">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="d288a-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="d288a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d288a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d288a-116">Not supported.</span></span>    |
|<span data-ttu-id="d288a-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="d288a-117">Application</span></span> | <span data-ttu-id="d288a-118">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="d288a-118">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d288a-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="d288a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="d288a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="d288a-120">Request headers</span></span>
| <span data-ttu-id="d288a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="d288a-121">Name</span></span>      |<span data-ttu-id="d288a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d288a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d288a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="d288a-123">Authorization</span></span>  | <span data-ttu-id="d288a-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="d288a-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d288a-126">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d288a-126">Workbook-Session-Id</span></span>  | <span data-ttu-id="d288a-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="d288a-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d288a-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="d288a-129">Request body</span></span>
<span data-ttu-id="d288a-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="d288a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d288a-131">Ответ</span><span class="sxs-lookup"><span data-stu-id="d288a-131">Response</span></span>

<span data-ttu-id="d288a-132">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [леакедкредентиалсрискевент](../resources/leakedcredentialsriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="d288a-132">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d288a-133">Пример</span><span class="sxs-lookup"><span data-stu-id="d288a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d288a-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="d288a-134">Request</span></span>
<span data-ttu-id="d288a-135">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="d288a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="d288a-136">Отклик</span><span class="sxs-lookup"><span data-stu-id="d288a-136">Response</span></span>
<span data-ttu-id="d288a-p105">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="d288a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value":
  [
    {
      "closedDateTime": null,
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "active",
      "riskLevel": "high",
      "riskType": "LeakedCredentialsRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "278dc452-4163-dbc6-84eb-a050c37fc931",
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
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
