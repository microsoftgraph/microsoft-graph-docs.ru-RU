---
title: Получение connectorGroup
description: Получение свойств объекта Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 996ed42380d6e6fd9ce301c5a622411281ebb15a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47982306"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="85509-103">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="85509-103">Get connectorGroup</span></span>

<span data-ttu-id="85509-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85509-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85509-105">Получение свойств объекта [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="85509-105">Retrieve the properties of a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="85509-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85509-106">Permissions</span></span>
<span data-ttu-id="85509-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85509-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85509-109">Permission type</span></span>      | <span data-ttu-id="85509-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85509-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85509-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85509-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85509-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85509-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="85509-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85509-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85509-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85509-114">Not supported.</span></span>    |
|<span data-ttu-id="85509-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85509-115">Application</span></span> | <span data-ttu-id="85509-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85509-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="85509-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85509-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="85509-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="85509-118">Optional query parameters</span></span>
<span data-ttu-id="85509-119">Этот метод поддерживает [параметры запросов OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="85509-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="85509-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85509-120">Request headers</span></span>
| <span data-ttu-id="85509-121">Имя</span><span class="sxs-lookup"><span data-stu-id="85509-121">Name</span></span>      |<span data-ttu-id="85509-122">Описание</span><span class="sxs-lookup"><span data-stu-id="85509-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="85509-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="85509-123">Authorization</span></span>  | <span data-ttu-id="85509-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="85509-124">Bearer.</span></span> <span data-ttu-id="85509-125">Обязательно</span><span class="sxs-lookup"><span data-stu-id="85509-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="85509-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="85509-126">Request body</span></span>
<span data-ttu-id="85509-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="85509-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="85509-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="85509-128">Response</span></span>

<span data-ttu-id="85509-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85509-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85509-130">Пример</span><span class="sxs-lookup"><span data-stu-id="85509-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="85509-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="85509-131">Request</span></span>
<span data-ttu-id="85509-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85509-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85509-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="85509-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="85509-134">C#</span><span class="sxs-lookup"><span data-stu-id="85509-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="85509-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85509-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="85509-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="85509-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="85509-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="85509-137">Response</span></span>
<span data-ttu-id="85509-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="85509-138">The following is an example of the response.</span></span> <span data-ttu-id="85509-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="85509-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="85509-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85509-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


