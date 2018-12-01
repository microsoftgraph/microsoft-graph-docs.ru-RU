---
title: Получение leakedCredentialsRiskEvent
description: Извлечение свойств и связи объекта leakedcredentialsriskevent.
ms.openlocfilehash: a3d259f785d2c8d6717f4dfe90ba04aeb454a1bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27082189"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="fece6-103">Получение leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="fece6-103">Get leakedCredentialsRiskEvent</span></span>

> <span data-ttu-id="fece6-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fece6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fece6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fece6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fece6-106">Извлечение свойств и связи объекта leakedcredentialsriskevent.</span><span class="sxs-lookup"><span data-stu-id="fece6-106">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="fece6-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fece6-107">Permissions</span></span>
<span data-ttu-id="fece6-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fece6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fece6-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fece6-110">Permission type</span></span>      | <span data-ttu-id="fece6-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fece6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fece6-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fece6-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fece6-113">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="fece6-113">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="fece6-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fece6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fece6-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fece6-115">Not supported.</span></span>    |
|<span data-ttu-id="fece6-116">Для приложения</span><span class="sxs-lookup"><span data-stu-id="fece6-116">Application</span></span> | <span data-ttu-id="fece6-117">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="fece6-117">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fece6-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fece6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="fece6-119">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fece6-119">Request headers</span></span>
| <span data-ttu-id="fece6-120">Имя</span><span class="sxs-lookup"><span data-stu-id="fece6-120">Name</span></span>      |<span data-ttu-id="fece6-121">Описание</span><span class="sxs-lookup"><span data-stu-id="fece6-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fece6-122">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fece6-122">Authorization</span></span>  | <span data-ttu-id="fece6-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="fece6-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fece6-125">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="fece6-125">Workbook-Session-Id</span></span>  | <span data-ttu-id="fece6-p104">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="fece6-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fece6-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="fece6-128">Request body</span></span>
<span data-ttu-id="fece6-129">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="fece6-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fece6-130">Ответ</span><span class="sxs-lookup"><span data-stu-id="fece6-130">Response</span></span>

<span data-ttu-id="fece6-131">Успешно завершена, этот метод возвращает `200 OK` объект [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) и кода ответа в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="fece6-131">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fece6-132">Пример</span><span class="sxs-lookup"><span data-stu-id="fece6-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fece6-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="fece6-133">Request</span></span>
<span data-ttu-id="fece6-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fece6-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="fece6-135">Ответ</span><span class="sxs-lookup"><span data-stu-id="fece6-135">Response</span></span>
<span data-ttu-id="fece6-p105">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="fece6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.leakedCredentialsRiskEvent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

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
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
