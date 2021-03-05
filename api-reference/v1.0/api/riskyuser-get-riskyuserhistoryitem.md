---
title: Получить историю
description: Ознакомьтесь с свойствами и отношениями объекта riskyUserHistoryItem.
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ef1baa85f405ffdb36ec86d97df858d864ead3cb
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440075"
---
# <a name="get-history"></a><span data-ttu-id="719ec-103">Получить историю</span><span class="sxs-lookup"><span data-stu-id="719ec-103">Get history</span></span>
<span data-ttu-id="719ec-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="719ec-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="719ec-105">Ознакомьтесь с свойствами и отношениями объекта [riskyUserHistoryItem.](../resources/riskyuserhistoryitem.md)</span><span class="sxs-lookup"><span data-stu-id="719ec-105">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>


><span data-ttu-id="719ec-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="719ec-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="719ec-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="719ec-107">Permissions</span></span>
<span data-ttu-id="719ec-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="719ec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="719ec-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="719ec-110">Permission type</span></span>      | <span data-ttu-id="719ec-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="719ec-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="719ec-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="719ec-112">Delegated (work or school account)</span></span> | <span data-ttu-id="719ec-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="719ec-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="719ec-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="719ec-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="719ec-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="719ec-115">Not supported.</span></span>    |
|<span data-ttu-id="719ec-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="719ec-116">Application</span></span> | <span data-ttu-id="719ec-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="719ec-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="719ec-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="719ec-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{userId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="719ec-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="719ec-119">Optional query parameters</span></span>
<span data-ttu-id="719ec-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="719ec-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="719ec-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="719ec-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="719ec-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="719ec-122">Request headers</span></span>
|<span data-ttu-id="719ec-123">Имя</span><span class="sxs-lookup"><span data-stu-id="719ec-123">Name</span></span>|<span data-ttu-id="719ec-124">Описание</span><span class="sxs-lookup"><span data-stu-id="719ec-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="719ec-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="719ec-125">Authorization</span></span>|<span data-ttu-id="719ec-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="719ec-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="719ec-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="719ec-128">Request body</span></span>
<span data-ttu-id="719ec-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="719ec-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="719ec-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="719ec-130">Response</span></span>

<span data-ttu-id="719ec-131">В случае успешной работы этот метод возвращает код ответа и объект `200 OK` [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="719ec-131">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="719ec-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="719ec-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="719ec-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="719ec-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```


### <a name="response"></a><span data-ttu-id="719ec-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="719ec-134">Response</span></span>
<span data-ttu-id="719ec-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="719ec-135">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.riskyUserHistoryItem"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": 
  {
    "@odata.type": "#microsoft.graph.riskyUserHistoryItem",
    "id": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "isDeleted": false,
    "isGuest": false,
    "isProcessing": false,
    "riskLevel": "none",
    "riskState": "remediated",
    "riskDetail": "userPerformedSecuredPasswordReset",
    "riskLastUpdatedDateTime": "2019-05-03T03:50:34.9565578Z",
    "userDisplayName": "Allan Deyoung",
    "userPrincipalName": "AllanD@contoso.OnMicrosoft.com",
    "userId": "41a31b00-3b3b-42d9-8f1c-6d4f14e74c69",
    "initiatedBy": "68ca8ec0-11f8-456b-a785-70d9936650d5",
    "activity": {
      "@odata.type": "microsoft.graph.riskUserActivity"
    }
  }
}
```


