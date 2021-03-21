---
title: Список ежемесячныхPrintUsageByUser
description: Извлечение списка ежемесячных сводок использования печати, сгруппив их пользователем.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: dba792f68284acb6db514af88d999d91c83af9ba
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50959580"
---
# <a name="list-monthlyprintusagebyuser"></a><span data-ttu-id="a6ee4-103">Список ежемесячныхPrintUsageByUser</span><span class="sxs-lookup"><span data-stu-id="a6ee4-103">List monthlyPrintUsageByUser</span></span>
<span data-ttu-id="a6ee4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6ee4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a6ee4-105">Извлечение списка ежемесячных сводок использования печати, сгруппив их пользователем.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-105">Retrieve a list of monthly print usage summaries, grouped by user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6ee4-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="a6ee4-106">Permissions</span></span>
<span data-ttu-id="a6ee4-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6ee4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a6ee4-109">Помимо следующих разрешений, клиент пользователя должен иметь активную подписку на универсальную печать.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="a6ee4-110">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="a6ee4-110">Permission type</span></span> | <span data-ttu-id="a6ee4-111">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="a6ee4-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a6ee4-112">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="a6ee4-112">Delegated (work or school account)</span></span>| <span data-ttu-id="a6ee4-113">Reports.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6ee4-113">Reports.Read.All</span></span> |
|<span data-ttu-id="a6ee4-114">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="a6ee4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6ee4-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-115">Not Supported.</span></span>|
|<span data-ttu-id="a6ee4-116">Для приложений</span><span class="sxs-lookup"><span data-stu-id="a6ee4-116">Application</span></span>|<span data-ttu-id="a6ee4-117">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6ee4-118">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="a6ee4-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /reports/monthlyPrintUsageByUser
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a6ee4-119">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="a6ee4-119">Optional query parameters</span></span>
<span data-ttu-id="a6ee4-120">Этот метод поддерживает некоторые параметры запросов OData для настройки отклика.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a6ee4-121">Общие сведения см. в статье [Параметры запроса OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="a6ee4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a6ee4-122">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="a6ee4-122">Request headers</span></span>
|<span data-ttu-id="a6ee4-123">Имя</span><span class="sxs-lookup"><span data-stu-id="a6ee4-123">Name</span></span>|<span data-ttu-id="a6ee4-124">Описание</span><span class="sxs-lookup"><span data-stu-id="a6ee4-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a6ee4-125">Авторизация</span><span class="sxs-lookup"><span data-stu-id="a6ee4-125">Authorization</span></span>|<span data-ttu-id="a6ee4-p103">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6ee4-128">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="a6ee4-128">Request body</span></span>
<span data-ttu-id="a6ee4-129">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a6ee4-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6ee4-130">Response</span></span>

<span data-ttu-id="a6ee4-131">В случае успешной работы этот метод возвращает код отклика и коллекцию `200 OK` [объектов printUsageByUser](../resources/printusagebyuser.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-131">If successful, this method returns a `200 OK` response code and a collection of [printUsageByUser](../resources/printusagebyuser.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6ee4-132">Примеры</span><span class="sxs-lookup"><span data-stu-id="a6ee4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6ee4-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="a6ee4-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a6ee4-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6ee4-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_printusagebyuser_2"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/reports/monthlyPrintUsageByUser
```
# <a name="c"></a>[<span data-ttu-id="a6ee4-135">C#</span><span class="sxs-lookup"><span data-stu-id="a6ee4-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-printusagebyuser-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6ee4-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6ee4-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-printusagebyuser-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6ee4-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6ee4-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-printusagebyuser-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a6ee4-138">Java</span><span class="sxs-lookup"><span data-stu-id="a6ee4-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-printusagebyuser-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a6ee4-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="a6ee4-139">Response</span></span>
<span data-ttu-id="a6ee4-140">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="a6ee4-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.printUsageByUser)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "userPrincipalName": "username@contoso.com",
      "usageDate": "Date",
      "completedBlackAndWhiteJobCount": 42,
      "completedColorJobCount": 0,
      "incompleteJobCount": 6
    }
  ]
}
```

