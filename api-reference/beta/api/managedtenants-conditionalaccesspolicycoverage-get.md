---
title: Get conditionalAccessPolicyCoverage
description: Ознакомьтесь с свойствами и отношениями объекта conditionalAccessPolicyCoverage.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0283b41d7576cef1228861db168dbd5e3a3bb511
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402484"
---
# <a name="get-conditionalaccesspolicycoverage"></a><span data-ttu-id="e3203-103">Get conditionalAccessPolicyCoverage</span><span class="sxs-lookup"><span data-stu-id="e3203-103">Get conditionalAccessPolicyCoverage</span></span>
<span data-ttu-id="e3203-104">Пространство имен: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="e3203-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3203-105">Ознакомьтесь с свойствами и отношениями объекта [conditionalAccessPolicyCoverage.](../resources/managedtenants-conditionalaccesspolicycoverage.md)</span><span class="sxs-lookup"><span data-stu-id="e3203-105">Read the properties and relationships of a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="e3203-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e3203-106">Permissions</span></span>
<span data-ttu-id="e3203-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3203-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3203-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e3203-109">Permission type</span></span>|<span data-ttu-id="e3203-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e3203-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3203-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e3203-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3203-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess и Application.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3203-112">Policy.Read.All, Policy.ReadWrite.ConditionalAccess, and Application.Read.All</span></span>|
|<span data-ttu-id="e3203-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e3203-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3203-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3203-114">Not supported.</span></span>|
|<span data-ttu-id="e3203-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e3203-115">Application</span></span>|<span data-ttu-id="e3203-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e3203-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3203-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e3203-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3203-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e3203-118">Optional query parameters</span></span>
<span data-ttu-id="e3203-119">Этот метод поддерживает параметры [запроса OData,](/graph/query-parameters) чтобы помочь настроить ответ, в том числе `$apply` , , , , , , , и `$count` `$filter` `$orderBy` `$select` `$skip` `$top` .</span><span class="sxs-lookup"><span data-stu-id="e3203-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3203-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e3203-120">Request headers</span></span>
|<span data-ttu-id="e3203-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e3203-121">Name</span></span>|<span data-ttu-id="e3203-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e3203-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e3203-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e3203-123">Authorization</span></span>|<span data-ttu-id="e3203-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e3203-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3203-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e3203-126">Request body</span></span>
<span data-ttu-id="e3203-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e3203-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3203-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3203-128">Response</span></span>

<span data-ttu-id="e3203-129">В случае успешной работы этот метод возвращает код ответа и `200 OK` [объект conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) в теле ответа.</span><span class="sxs-lookup"><span data-stu-id="e3203-129">If successful, this method returns a `200 OK` response code and a [conditionalAccessPolicyCoverage](../resources/managedtenants-conditionalaccesspolicycoverage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e3203-130">Примеры</span><span class="sxs-lookup"><span data-stu-id="e3203-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e3203-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e3203-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_conditionalaccesspolicycoverage"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/conditionalAccessPolicyCoverages/{conditionalAccessPolicyCoverageId}
```


### <a name="response"></a><span data-ttu-id="e3203-132">Отклик</span><span class="sxs-lookup"><span data-stu-id="e3203-132">Response</span></span>
><span data-ttu-id="e3203-133">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="e3203-133">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.conditionalAccessPolicyCoverage"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.conditionalAccessPolicyCoverage",
  "id": "38227791-a88b-4fcc-81c5-58cf77668320",
  "conditionalAccessPolicyState": "enabled",
  "requiresDeviceCompliance": false,
  "latestPolicyModifiedDateTime": "2021-07-11T14:56:13.598304Z",
  "tenantDisplayName": "Consolidated Messenger"
}
```
