---
title: Получение журнала
description: Чтение свойств и связей объекта Рискюсерхисторитем.
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 141aaa6a1c0642159cccfe075aa8934fa65883cd
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897577"
---
# <a name="get-history"></a><span data-ttu-id="5ad0c-103">Получение журнала</span><span class="sxs-lookup"><span data-stu-id="5ad0c-103">Get history</span></span>
<span data-ttu-id="5ad0c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ad0c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ad0c-105">Чтение свойств и связей объекта [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) .</span><span class="sxs-lookup"><span data-stu-id="5ad0c-105">Read the properties and relationships of a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object.</span></span>


><span data-ttu-id="5ad0c-106">**Примечание:** Для использования API riskyUsers требуется лицензия Azure AD Premium P2.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-106">**Note:** Using the riskyUsers API requires an Azure AD Premium P2 license.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ad0c-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="5ad0c-107">Permissions</span></span>
<span data-ttu-id="5ad0c-108">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-108">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="5ad0c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="5ad0c-109">To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

|<span data-ttu-id="5ad0c-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="5ad0c-110">Permission type</span></span>      | <span data-ttu-id="5ad0c-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="5ad0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ad0c-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="5ad0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ad0c-113">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5ad0c-113">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span>    |
|<span data-ttu-id="5ad0c-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="5ad0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ad0c-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-115">Not supported.</span></span>    |
|<span data-ttu-id="5ad0c-116">Приложение</span><span class="sxs-lookup"><span data-stu-id="5ad0c-116">Application</span></span> | <span data-ttu-id="5ad0c-117">Идентитирискюсер. Read. ALL, Идентитирискусер. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="5ad0c-117">IdentityRiskyUser.Read.All, IdentityRiskUser.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ad0c-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="5ad0c-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /identityProtection/riskyUsers/{userId}/history
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ad0c-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="5ad0c-119">Optional query parameters</span></span>
<span data-ttu-id="5ad0c-120">Этот метод поддерживает некоторые параметры запроса OData для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5ad0c-121">Общие сведения можно найти в разделе [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="5ad0c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ad0c-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="5ad0c-122">Request headers</span></span>
|<span data-ttu-id="5ad0c-123">Имя</span><span class="sxs-lookup"><span data-stu-id="5ad0c-123">Name</span></span>|<span data-ttu-id="5ad0c-124">Описание</span><span class="sxs-lookup"><span data-stu-id="5ad0c-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ad0c-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="5ad0c-125">Authorization</span></span>|<span data-ttu-id="5ad0c-126">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-126">Bearer {token}.</span></span> <span data-ttu-id="5ad0c-127">Required.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-127">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ad0c-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="5ad0c-128">Request body</span></span>
<span data-ttu-id="5ad0c-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ad0c-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ad0c-130">Response</span></span>

<span data-ttu-id="5ad0c-131">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [рискюсерхисторитем](../resources/riskyuserhistoryitem.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-131">If successful, this method returns a `200 OK` response code and a [riskyUserHistoryItem](../resources/riskyuserhistoryitem.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ad0c-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="5ad0c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ad0c-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="5ad0c-133">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_riskyuserhistoryitem"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/identityProtection/riskyUsers/41a31b00-3b3b-42d9-8f1c-6d4f14e74c69/history
```


### <a name="response"></a><span data-ttu-id="5ad0c-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="5ad0c-134">Response</span></span>
<span data-ttu-id="5ad0c-135">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="5ad0c-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

