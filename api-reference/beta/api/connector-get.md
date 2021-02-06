---
title: Получение соединителя
description: Извлечение свойств объекта соединители.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 84d3d5d3b2ae8375304844e5d88315896722d110
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130096"
---
# <a name="get-connector"></a><span data-ttu-id="3d502-103">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="3d502-103">Get connector</span></span>

<span data-ttu-id="3d502-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d502-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d502-105">Извлечение свойств и [](../resources/connector.md) связей объекта соединители.</span><span class="sxs-lookup"><span data-stu-id="3d502-105">Retrieve the properties and relationships of a [connector](../resources/connector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d502-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="3d502-106">Permissions</span></span>
<span data-ttu-id="3d502-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3d502-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d502-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="3d502-109">Permission type</span></span>      | <span data-ttu-id="3d502-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="3d502-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d502-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="3d502-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3d502-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3d502-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3d502-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="3d502-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d502-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d502-114">Not supported.</span></span>    |
|<span data-ttu-id="3d502-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="3d502-115">Application</span></span> | <span data-ttu-id="3d502-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3d502-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="3d502-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="3d502-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3d502-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="3d502-118">Optional query parameters</span></span>
<span data-ttu-id="3d502-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="3d502-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3d502-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="3d502-120">Request headers</span></span>
| <span data-ttu-id="3d502-121">Имя</span><span class="sxs-lookup"><span data-stu-id="3d502-121">Name</span></span>      |<span data-ttu-id="3d502-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3d502-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3d502-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="3d502-123">Authorization</span></span>  | <span data-ttu-id="3d502-124">Bearer.</span><span class="sxs-lookup"><span data-stu-id="3d502-124">Bearer.</span></span> <span data-ttu-id="3d502-125">Обязательна</span><span class="sxs-lookup"><span data-stu-id="3d502-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d502-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="3d502-126">Request body</span></span>
<span data-ttu-id="3d502-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="3d502-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3d502-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d502-128">Response</span></span>

<span data-ttu-id="3d502-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` соединители [](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="3d502-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d502-130">Пример</span><span class="sxs-lookup"><span data-stu-id="3d502-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3d502-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="3d502-131">Request</span></span>

<span data-ttu-id="3d502-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="3d502-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3d502-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3d502-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="3d502-134">C#</span><span class="sxs-lookup"><span data-stu-id="3d502-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3d502-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3d502-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3d502-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3d502-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3d502-137">Java</span><span class="sxs-lookup"><span data-stu-id="3d502-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="3d502-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="3d502-138">Response</span></span>
<span data-ttu-id="3d502-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="3d502-139">The following is an example of the response.</span></span> <span data-ttu-id="3d502-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="3d502-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3d502-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="3d502-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

