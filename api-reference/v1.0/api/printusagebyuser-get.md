---
title: Get printUsageByUser
description: Извлечение сводки об использовании пользователя за определенный период времени.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 10a3ee5b83d2f07d9b2407f26f3b7fa210786a1c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774407"
---
# <a name="get-printusagebyuser"></a><span data-ttu-id="df083-103">Get printUsageByUser</span><span class="sxs-lookup"><span data-stu-id="df083-103">Get printUsageByUser</span></span>
<span data-ttu-id="df083-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df083-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="df083-105">Извлечение сводки об использовании пользователя за определенный период времени.</span><span class="sxs-lookup"><span data-stu-id="df083-105">Retrieve a user's usage summary for a particular time period.</span></span> <span data-ttu-id="df083-106">Описание каждой конечной точки см. в [printUsageByUser.](../resources/printUsageByUser.md)</span><span class="sxs-lookup"><span data-stu-id="df083-106">For descriptions of each endpoint, see [printUsageByUser](../resources/printUsageByUser.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="df083-107">Разрешения</span><span class="sxs-lookup"><span data-stu-id="df083-107">Permissions</span></span>
<span data-ttu-id="df083-p102">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="df083-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="df083-110">Чтобы использовать службу универсальной печати, пользователь или клиент приложения должен иметь активную подписку универсальной печати в дополнение к разрешениям, перечисленным в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="df083-110">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span>

|<span data-ttu-id="df083-111">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="df083-111">Permission type</span></span> | <span data-ttu-id="df083-112">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="df083-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="df083-113">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="df083-113">Delegated (work or school account)</span></span>| <span data-ttu-id="df083-114">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="df083-114">Reports.Read.All</span></span> |
|<span data-ttu-id="df083-115">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="df083-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df083-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df083-116">Not Supported.</span></span>|
|<span data-ttu-id="df083-117">Для приложений</span><span class="sxs-lookup"><span data-stu-id="df083-117">Application</span></span>|<span data-ttu-id="df083-118">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="df083-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df083-119">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="df083-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/dailyPrintUsageByUser/{id}
GET /reports/monthlyPrintUsageByUser/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="df083-120">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="df083-120">Optional query parameters</span></span>
<span data-ttu-id="df083-121">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="df083-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="df083-122">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="df083-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="df083-123">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="df083-123">Request headers</span></span>
|<span data-ttu-id="df083-124">Имя</span><span class="sxs-lookup"><span data-stu-id="df083-124">Name</span></span>|<span data-ttu-id="df083-125">Описание</span><span class="sxs-lookup"><span data-stu-id="df083-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="df083-126">Авторизация</span><span class="sxs-lookup"><span data-stu-id="df083-126">Authorization</span></span>|<span data-ttu-id="df083-p104">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="df083-p104">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df083-129">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="df083-129">Request body</span></span>
<span data-ttu-id="df083-130">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="df083-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df083-131">Отклик</span><span class="sxs-lookup"><span data-stu-id="df083-131">Response</span></span>

<span data-ttu-id="df083-132">В случае успешной работы этот метод возвращает код отклика и `200 OK` [объект printUsageByUser](../resources/printusagebyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="df083-132">If successful, this method returns a `200 OK` response code and a [printUsageByUser](../resources/printusagebyuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="df083-133">Примеры</span><span class="sxs-lookup"><span data-stu-id="df083-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="df083-134">Запрос</span><span class="sxs-lookup"><span data-stu-id="df083-134">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="df083-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="df083-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_printusagebyuser"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/dailyPrintUsageByUser/{id}
```
# <a name="c"></a>[<span data-ttu-id="df083-136">C#</span><span class="sxs-lookup"><span data-stu-id="df083-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-printusagebyuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df083-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df083-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-printusagebyuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df083-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df083-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-printusagebyuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df083-139">Java</span><span class="sxs-lookup"><span data-stu-id="df083-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-printusagebyuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="df083-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="df083-140">Response</span></span>
<span data-ttu-id="df083-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="df083-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printUsageByUser"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "userPrincipalName": "username@contoso.com",
  "usageDate": "Date",
  "completedBlackAndWhiteJobCount": 42,
  "completedColorJobCount": 0,
  "incompleteJobCount": 6
}
```

