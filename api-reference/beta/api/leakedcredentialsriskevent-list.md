---
title: Список leakedCredentialsRiskEvents
description: Получение списка объектов leakedcredentialsriskevent.
ms.openlocfilehash: 49cfd54c580634e43cff50aa7c125ffc79116ea3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27079987"
---
# <a name="list-leakedcredentialsriskevents"></a><span data-ttu-id="71dfc-103">Список leakedCredentialsRiskEvents</span><span class="sxs-lookup"><span data-stu-id="71dfc-103">List leakedCredentialsRiskEvents</span></span>

> <span data-ttu-id="71dfc-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="71dfc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="71dfc-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71dfc-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="71dfc-106">Получение списка объектов leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="71dfc-106">Retrieve a list of leakedcredentialsriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="71dfc-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="71dfc-107">Permissions</span></span>
<span data-ttu-id="71dfc-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="71dfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71dfc-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="71dfc-110">Permission type</span></span>      | <span data-ttu-id="71dfc-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="71dfc-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71dfc-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="71dfc-112">Delegated (work or school account)</span></span> | <span data-ttu-id="71dfc-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="71dfc-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="71dfc-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="71dfc-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71dfc-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="71dfc-115">Not supported.</span></span>    |
|<span data-ttu-id="71dfc-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="71dfc-116">Application</span></span> | <span data-ttu-id="71dfc-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="71dfc-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71dfc-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="71dfc-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="71dfc-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="71dfc-119">Request headers</span></span>
| <span data-ttu-id="71dfc-120">Имя</span><span class="sxs-lookup"><span data-stu-id="71dfc-120">Name</span></span>      |<span data-ttu-id="71dfc-121">Описание</span><span class="sxs-lookup"><span data-stu-id="71dfc-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="71dfc-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="71dfc-122">Authorization</span></span>  | <span data-ttu-id="71dfc-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="71dfc-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71dfc-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="71dfc-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="71dfc-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="71dfc-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="71dfc-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="71dfc-128">Request body</span></span>
<span data-ttu-id="71dfc-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="71dfc-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71dfc-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="71dfc-130">Response</span></span>

<span data-ttu-id="71dfc-131">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="71dfc-131">If successful, this method returns a `200 OK` response code and collection of [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71dfc-132">Пример</span><span class="sxs-lookup"><span data-stu-id="71dfc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71dfc-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="71dfc-133">Request</span></span>
<span data-ttu-id="71dfc-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="71dfc-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents
```
##### <a name="response"></a><span data-ttu-id="71dfc-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="71dfc-135">Response</span></span>
<span data-ttu-id="71dfc-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="71dfc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List leakedCredentialsRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
