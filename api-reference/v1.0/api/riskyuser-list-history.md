---
title: История списка
description: Получите свойство riskyUserHistoryItems из свойства навигации по истории.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 4115251bbc9644e4f3beb5fdf0ddea0437f6d594
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448069"
---
# <a name="list-history"></a><span data-ttu-id="0e8f5-103">История списка</span><span class="sxs-lookup"><span data-stu-id="0e8f5-103">List history</span></span>
<span data-ttu-id="0e8f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e8f5-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e8f5-105">Получите свойство riskyUserHistoryItems из свойства навигации по истории.</span><span class="sxs-lookup"><span data-stu-id="0e8f5-105">Get the riskyUserHistoryItems from the history navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="0e8f5-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="0e8f5-106">Permissions</span></span>
<span data-ttu-id="0e8f5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="0e8f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="0e8f5-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0e8f5-109">Permission type</span></span>|<span data-ttu-id="0e8f5-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0e8f5-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e8f5-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0e8f5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0e8f5-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e8f5-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="0e8f5-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0e8f5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e8f5-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0e8f5-114">Not supported.</span></span>    |
|<span data-ttu-id="0e8f5-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0e8f5-115">Application</span></span> | <span data-ttu-id="0e8f5-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="0e8f5-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e8f5-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0e8f5-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0e8f5-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="0e8f5-118">Optional query parameters</span></span>
<span data-ttu-id="0e8f5-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="0e8f5-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="0e8f5-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="0e8f5-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0e8f5-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0e8f5-121">Request headers</span></span>
|<span data-ttu-id="0e8f5-122">Имя</span><span class="sxs-lookup"><span data-stu-id="0e8f5-122">Name</span></span>|<span data-ttu-id="0e8f5-123">Описание</span><span class="sxs-lookup"><span data-stu-id="0e8f5-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0e8f5-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="0e8f5-124">Authorization</span></span>|<span data-ttu-id="0e8f5-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="0e8f5-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e8f5-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="0e8f5-127">Request body</span></span>
<span data-ttu-id="0e8f5-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="0e8f5-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0e8f5-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e8f5-129">Response</span></span>

<span data-ttu-id="0e8f5-130">В случае успешной работы этот метод возвращает код ответа и коллекцию объектов `200 OK` [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="0e8f5-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0e8f5-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="0e8f5-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0e8f5-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="0e8f5-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a><span data-ttu-id="0e8f5-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="0e8f5-133">Response</span></span>
<span data-ttu-id="0e8f5-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="0e8f5-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "collection(microsoft.graph.riskyUserHistoryItem)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
      "id": "5e1d812e-812e-5e1d-2e81-1d5e2e811d5e",
      "isDeleted": "Boolean",
      "isProcessing": "Boolean",
      "riskLastUpdatedDateTime": "String (timestamp)",
      "riskLevel": "String",
      "riskState": "String",
      "riskDetail": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userId": "String",
      "initiatedBy": "String",
      "activity": {
          "riskEventTypes": [],
          "detail": "userPerformedSecuredPasswordReset"
      }
    }
  ]
}
```


