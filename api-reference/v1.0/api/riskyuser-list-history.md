---
title: Журнал списка
description: Получение Рискюсерхисторитемс из свойства навигации по журналу.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1fcbe019d1aa673d100cedf5904b529960cec9b0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051335"
---
# <a name="list-history"></a><span data-ttu-id="bf351-103">Журнал списка</span><span class="sxs-lookup"><span data-stu-id="bf351-103">List history</span></span>
<span data-ttu-id="bf351-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf351-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bf351-105">Получение Рискюсерхисторитемс из свойства навигации по журналу.</span><span class="sxs-lookup"><span data-stu-id="bf351-105">Get the riskyUserHistoryItems from the history navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf351-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="bf351-106">Permissions</span></span>
<span data-ttu-id="bf351-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="bf351-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="bf351-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="bf351-109">Permission type</span></span>|<span data-ttu-id="bf351-110">Разрешения (в порядке убывания привилегий)</span><span class="sxs-lookup"><span data-stu-id="bf351-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bf351-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="bf351-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf351-112">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf351-112">IdentityRiskyUser.Read.All</span></span>    |
|<span data-ttu-id="bf351-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="bf351-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf351-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf351-114">Not supported.</span></span>    |
|<span data-ttu-id="bf351-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="bf351-115">Application</span></span> | <span data-ttu-id="bf351-116">IdentityRiskyUser.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf351-116">IdentityRiskyUser.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf351-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="bf351-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{riskyUserId}/history
GET /identityProtection/riskyUsers/{riskyUserId}/history/{riskyUserHistoryItemId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf351-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="bf351-118">Optional query parameters</span></span>
<span data-ttu-id="bf351-119">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="bf351-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="bf351-120">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="bf351-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf351-121">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="bf351-121">Request headers</span></span>
|<span data-ttu-id="bf351-122">Имя</span><span class="sxs-lookup"><span data-stu-id="bf351-122">Name</span></span>|<span data-ttu-id="bf351-123">Описание</span><span class="sxs-lookup"><span data-stu-id="bf351-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="bf351-124">Авторизация</span><span class="sxs-lookup"><span data-stu-id="bf351-124">Authorization</span></span>|<span data-ttu-id="bf351-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="bf351-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf351-127">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="bf351-127">Request body</span></span>
<span data-ttu-id="bf351-128">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="bf351-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf351-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf351-129">Response</span></span>

<span data-ttu-id="bf351-130">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и коллекцию объектов [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="bf351-130">If successful, this method returns a `200 OK` response code and a collection of [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="bf351-131">Примеры</span><span class="sxs-lookup"><span data-stu-id="bf351-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="bf351-132">Запрос</span><span class="sxs-lookup"><span data-stu-id="bf351-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/{riskyUserId}/history
```


### <a name="response"></a><span data-ttu-id="bf351-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="bf351-133">Response</span></span>
<span data-ttu-id="bf351-134">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="bf351-134">**Note:** The response object shown here might be shortened for readability.</span></span>
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


