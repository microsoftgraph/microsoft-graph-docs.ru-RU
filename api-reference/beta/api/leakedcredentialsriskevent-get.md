---
title: Получение объекта leakedCredentialsRiskEvent
description: Получение свойств и связей объекта леакедкредентиалсрискевент.
localization_priority: Normal
ms.openlocfilehash: 2fd58105111b7f04976881729e17d073e223ff52
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333542"
---
# <a name="get-leakedcredentialsriskevent"></a><span data-ttu-id="76569-103">Получение объекта leakedCredentialsRiskEvent</span><span class="sxs-lookup"><span data-stu-id="76569-103">Get leakedCredentialsRiskEvent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76569-104">Получение свойств и связей объекта леакедкредентиалсрискевент.</span><span class="sxs-lookup"><span data-stu-id="76569-104">Retrieve the properties and relationships of a leakedcredentialsriskevent object.</span></span>
## <a name="permissions"></a><span data-ttu-id="76569-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="76569-105">Permissions</span></span>
<span data-ttu-id="76569-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76569-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76569-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="76569-108">Permission type</span></span>      | <span data-ttu-id="76569-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="76569-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="76569-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="76569-110">Delegated (work or school account)</span></span> | <span data-ttu-id="76569-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="76569-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="76569-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="76569-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="76569-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76569-113">Not supported.</span></span>    |
|<span data-ttu-id="76569-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="76569-114">Application</span></span> | <span data-ttu-id="76569-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="76569-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="76569-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="76569-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /leakedCredentialsRiskEvents/{id}
```
## <a name="request-headers"></a><span data-ttu-id="76569-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="76569-117">Request headers</span></span>
| <span data-ttu-id="76569-118">Имя</span><span class="sxs-lookup"><span data-stu-id="76569-118">Name</span></span>      |<span data-ttu-id="76569-119">Описание</span><span class="sxs-lookup"><span data-stu-id="76569-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76569-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="76569-120">Authorization</span></span>  | <span data-ttu-id="76569-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="76569-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="76569-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="76569-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="76569-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="76569-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="76569-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="76569-126">Request body</span></span>
<span data-ttu-id="76569-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="76569-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76569-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="76569-128">Response</span></span>

<span data-ttu-id="76569-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [леакедкредентиалсрискевент](../resources/leakedcredentialsriskevent.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="76569-129">If successful, this method returns a `200 OK` response code and [leakedCredentialsRiskEvent](../resources/leakedcredentialsriskevent.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76569-130">Пример</span><span class="sxs-lookup"><span data-stu-id="76569-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76569-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="76569-131">Request</span></span>
<span data-ttu-id="76569-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="76569-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_leakedcredentialsriskevent"
}-->
```http
GET https://graph.microsoft.com/v1.0/leakedCredentialsRiskEvents/8c793a18-c86a-b5f9-7d9a-b3d024f33eee-278dc452-4163-dbc6-84eb-a050c37fc931-1a01abd3-b87a-cece-3f4d-c788b055c182
```
##### <a name="response"></a><span data-ttu-id="76569-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="76569-133">Response</span></span>
<span data-ttu-id="76569-p104">Ниже приведен пример ответа. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="76569-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get leakedCredentialsRiskEvent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
