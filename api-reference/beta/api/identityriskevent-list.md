---
title: Список identityRiskEvents
description: Получение списка объектов identityriskevent.
author: cloudhandler
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: a5f6bf6936cda127fdc10970182d05e036a321c7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528944"
---
# <a name="list-identityriskevents"></a><span data-ttu-id="9ccdb-103">Список identityRiskEvents</span><span class="sxs-lookup"><span data-stu-id="9ccdb-103">List identityRiskEvents</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ccdb-104">Получение списка объектов identityriskevent.</span><span class="sxs-lookup"><span data-stu-id="9ccdb-104">Retrieve a list of identityriskevent objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="9ccdb-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="9ccdb-105">Permissions</span></span>
<span data-ttu-id="9ccdb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9ccdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ccdb-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="9ccdb-108">Permission type</span></span>      | <span data-ttu-id="9ccdb-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="9ccdb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ccdb-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="9ccdb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9ccdb-111">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ccdb-111">IdentityRiskEvent.Read.All</span></span>    |
|<span data-ttu-id="9ccdb-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="9ccdb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ccdb-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9ccdb-113">Not supported.</span></span>    |
|<span data-ttu-id="9ccdb-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="9ccdb-114">Application</span></span> | <span data-ttu-id="9ccdb-115">IdentityRiskEvent.Read.All</span><span class="sxs-lookup"><span data-stu-id="9ccdb-115">IdentityRiskEvent.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ccdb-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="9ccdb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /identityRiskEvents
```
## <a name="request-headers"></a><span data-ttu-id="9ccdb-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="9ccdb-117">Request headers</span></span>
| <span data-ttu-id="9ccdb-118">Имя</span><span class="sxs-lookup"><span data-stu-id="9ccdb-118">Name</span></span>      |<span data-ttu-id="9ccdb-119">Описание</span><span class="sxs-lookup"><span data-stu-id="9ccdb-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ccdb-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="9ccdb-120">Authorization</span></span>  | <span data-ttu-id="9ccdb-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="9ccdb-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="9ccdb-123">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="9ccdb-123">Workbook-Session-Id</span></span>  | <span data-ttu-id="9ccdb-p103">Идентификатор сеанса работы с книгой, определяющий, сохраняются ли изменения. Задавать не обязательно.</span><span class="sxs-lookup"><span data-stu-id="9ccdb-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ccdb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="9ccdb-126">Request body</span></span>
<span data-ttu-id="9ccdb-127">Не указывайте тело запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="9ccdb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ccdb-128">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ccdb-128">Response</span></span>

<span data-ttu-id="9ccdb-129">Успешно завершена, этот метод возвращает `200 OK` код ответа и коллекцию объектов [identityRiskEvent](../resources/identityriskevent.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="9ccdb-129">If successful, this method returns a `200 OK` response code and collection of [identityRiskEvent](../resources/identityriskevent.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9ccdb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="9ccdb-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9ccdb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="9ccdb-131">Request</span></span>
<span data-ttu-id="9ccdb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="9ccdb-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_identityriskevents"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityRiskEvents
```
##### <a name="response"></a><span data-ttu-id="9ccdb-133">Ответ</span><span class="sxs-lookup"><span data-stu-id="9ccdb-133">Response</span></span>
<span data-ttu-id="9ccdb-p104">Ниже приведен пример ответа. Примечание. Объект ответа, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.
</span><span class="sxs-lookup"><span data-stu-id="9ccdb-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityRiskEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 304

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.malwareRiskEvent",
      "malwareName": "CONFICKER",
      "closedDateTime": null,
      "createdDateTime": "2016-02-03T06:06:01.940814Z",
      "deviceInformation": "B62XYZ13OX",
      "id": "74ceb0af-2271-9167-ffa0-b6ac3b4e8781-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-0fdc2304-ba4c-ac0c-bdd7-da2d10e93849",
      "ipAddress": "95.31.18.119",
      "location": "Moskva, Russia, RU",
      "riskEventDateTime": "2016-02-03T05:20:33.7208156Z",
      "riskEventStatus": "active",
      "riskLevel": "low",
      "riskType": "MalwareRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
      "userPrincipalName": "jon@contoso.com"
    },
    {
      "@odata.type": "#microsoft.graph.unfamiliarLocationRiskEvent",
      "closedDateTime": "2016-01-29T20:03:57.7872426Z",
      "createdDateTime": "2016-01-29T00:01:49.126468Z",
      "id": "ec50e9fb-9da1-215b-e18c-b7e2a716b2a6-9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89-db69711e-9324-ec99-f010-6e63fb972e98",
      "ipAddress": "176.10.104.240",
      "location": "Bern, CH",
      "riskEventDateTime": "2016-01-29T00:00:56.2255665Z",
      "riskEventStatus": "remediated",
      "riskLevel": "medium",
      "riskType": "UnfamiliarLocationRiskEvent",
      "userDisplayName": "Jon Doe",
      "userId": "9eaaa2e3-4681-ae31-1eb6-7e46ae11ac89",
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
  "description": "List identityRiskEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/identityriskevent-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
