---
title: Перечисление соединителей
description: Извлечение списка объектов соединители.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 27fb3343b230d3397809063da1d8f56cf80ac9c3
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50947144"
---
# <a name="list-connectors"></a><span data-ttu-id="dc3eb-103">Перечисление соединителей</span><span class="sxs-lookup"><span data-stu-id="dc3eb-103">List connectors</span></span>

<span data-ttu-id="dc3eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc3eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc3eb-105">Извлечение списка [объектов соединители.](../resources/connector.md)</span><span class="sxs-lookup"><span data-stu-id="dc3eb-105">Retrieve a list of [connector](../resources/connector.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc3eb-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dc3eb-106">Permissions</span></span>
<span data-ttu-id="dc3eb-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dc3eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc3eb-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dc3eb-109">Permission type</span></span>      | <span data-ttu-id="dc3eb-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dc3eb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc3eb-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dc3eb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc3eb-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc3eb-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dc3eb-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dc3eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc3eb-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-114">Not supported.</span></span>    |
|<span data-ttu-id="dc3eb-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dc3eb-115">Application</span></span> | <span data-ttu-id="dc3eb-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc3eb-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dc3eb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dc3eb-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dc3eb-118">Optional query parameters</span></span>
<span data-ttu-id="dc3eb-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dc3eb-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dc3eb-120">Request headers</span></span>
| <span data-ttu-id="dc3eb-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dc3eb-121">Name</span></span>      |<span data-ttu-id="dc3eb-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dc3eb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dc3eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc3eb-123">Authorization</span></span>  | <span data-ttu-id="dc3eb-124">Носителер.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-124">Bearer.</span></span> <span data-ttu-id="dc3eb-125">Обязательный</span><span class="sxs-lookup"><span data-stu-id="dc3eb-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc3eb-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dc3eb-126">Request body</span></span>
<span data-ttu-id="dc3eb-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc3eb-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc3eb-128">Response</span></span>

<span data-ttu-id="dc3eb-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [соединителов](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-129">If successful, this method returns a `200 OK` response code and collection of [connector](../resources/connector.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc3eb-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dc3eb-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="dc3eb-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dc3eb-131">Request</span></span>
<span data-ttu-id="dc3eb-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc3eb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc3eb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectors_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors
```
# <a name="c"></a>[<span data-ttu-id="dc3eb-134">C#</span><span class="sxs-lookup"><span data-stu-id="dc3eb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectors-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc3eb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc3eb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectors-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc3eb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc3eb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectors-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc3eb-137">Java</span><span class="sxs-lookup"><span data-stu-id="dc3eb-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectors-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dc3eb-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dc3eb-138">Response</span></span>
<span data-ttu-id="dc3eb-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-139">The following is an example of the response.</span></span> <span data-ttu-id="dc3eb-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="dc3eb-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="dc3eb-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 169

{
  "value": [
    {
      "id": "id-value",
      "machineName": "machineName-value",
      "externalIp": "externalIp-value",
      "status": "status-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectors",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

