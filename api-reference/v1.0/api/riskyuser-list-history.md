---
title: Журнал списка
description: Получение Рискюсерхисторитемс из свойства навигации по журналу.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 212f10e5794a55dec925d1ec32c37abf9708700b
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897563"
---
# <a name="list-history"></a><span data-ttu-id="3fcde-103">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="3fcde-103">List history</span></span>
<span data-ttu-id="3fcde-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3fcde-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3fcde-105">Получение Рискюсерхисторитемс из свойства навигации по журналу.</span><span class="sxs-lookup"><span data-stu-id="3fcde-105">Get the riskyUserHistoryItems from the history navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="3fcde-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3fcde-106">Permissions</span></span>
<span data-ttu-id="3fcde-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="3fcde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="3fcde-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3fcde-109">Permission type</span></span>|<span data-ttu-id="3fcde-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="3fcde-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3fcde-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3fcde-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3fcde-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fcde-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="3fcde-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3fcde-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3fcde-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3fcde-114">Not supported.</span></span>    |
|<span data-ttu-id="3fcde-115">Приложение</span><span class="sxs-lookup"><span data-stu-id="3fcde-115">Application</span></span> | <span data-ttu-id="3fcde-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="3fcde-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3fcde-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3fcde-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3fcde-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3fcde-118">Optional query parameters</span></span>
<span data-ttu-id="3fcde-119">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3fcde-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3fcde-120">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3fcde-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3fcde-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3fcde-121">Request headers</span></span>
|<span data-ttu-id="3fcde-122">Имя</span><span class="sxs-lookup"><span data-stu-id="3fcde-122">Name</span></span>|<span data-ttu-id="3fcde-123">Описание</span><span class="sxs-lookup"><span data-stu-id="3fcde-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3fcde-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3fcde-124">Authorization</span></span>|<span data-ttu-id="3fcde-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="3fcde-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3fcde-127">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3fcde-127">Request body</span></span>
<span data-ttu-id="3fcde-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3fcde-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3fcde-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fcde-129">Response</span></span>

<span data-ttu-id="3fcde-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3fcde-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3fcde-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="3fcde-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3fcde-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="3fcde-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a><span data-ttu-id="3fcde-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="3fcde-133">Response</span></span>
<span data-ttu-id="3fcde-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3fcde-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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

