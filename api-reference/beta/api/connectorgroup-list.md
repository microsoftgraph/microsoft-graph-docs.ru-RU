---
title: Перечисление connectorGroups
description: Получить список объектов connectorgroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 7d8ad142840abba411fb6f2c3b9f0f49c55acd56
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130103"
---
# <a name="list-connectorgroups"></a><span data-ttu-id="aaca8-103">Перечисление connectorGroups</span><span class="sxs-lookup"><span data-stu-id="aaca8-103">List connectorGroups</span></span>

<span data-ttu-id="aaca8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaca8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaca8-105">Получить список объектов [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="aaca8-105">Retrieve a list of [connectorGroup](../resources/connectorgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaca8-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="aaca8-106">Permissions</span></span>
<span data-ttu-id="aaca8-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="aaca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aaca8-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="aaca8-109">Permission type</span></span>      | <span data-ttu-id="aaca8-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="aaca8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aaca8-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="aaca8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aaca8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="aaca8-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="aaca8-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="aaca8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaca8-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaca8-114">Not supported.</span></span>    |
|<span data-ttu-id="aaca8-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="aaca8-115">Application</span></span> | <span data-ttu-id="aaca8-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="aaca8-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaca8-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="aaca8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="aaca8-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="aaca8-118">Optional query parameters</span></span>
<span data-ttu-id="aaca8-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="aaca8-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaca8-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="aaca8-120">Request headers</span></span>
| <span data-ttu-id="aaca8-121">Имя</span><span class="sxs-lookup"><span data-stu-id="aaca8-121">Name</span></span>      |<span data-ttu-id="aaca8-122">Описание</span><span class="sxs-lookup"><span data-stu-id="aaca8-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="aaca8-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="aaca8-123">Authorization</span></span>  | <span data-ttu-id="aaca8-124">Bearer.</span><span class="sxs-lookup"><span data-stu-id="aaca8-124">Bearer.</span></span> <span data-ttu-id="aaca8-125">Обязательна</span><span class="sxs-lookup"><span data-stu-id="aaca8-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="aaca8-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="aaca8-126">Request body</span></span>
<span data-ttu-id="aaca8-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="aaca8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaca8-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaca8-128">Response</span></span>

<span data-ttu-id="aaca8-129">В случае успеха этот метод возвращает код отклика и коллекцию объектов `200 OK` [connectorGroup](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="aaca8-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aaca8-130">Пример</span><span class="sxs-lookup"><span data-stu-id="aaca8-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="aaca8-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="aaca8-131">Request</span></span>

<span data-ttu-id="aaca8-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="aaca8-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="aaca8-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaca8-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
```
# <a name="c"></a>[<span data-ttu-id="aaca8-134">C#</span><span class="sxs-lookup"><span data-stu-id="aaca8-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaca8-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaca8-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaca8-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaca8-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaca8-137">Java</span><span class="sxs-lookup"><span data-stu-id="aaca8-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectorgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="aaca8-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="aaca8-138">Response</span></span>
<span data-ttu-id="aaca8-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="aaca8-139">The following is an example of the response.</span></span> <span data-ttu-id="aaca8-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="aaca8-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="aaca8-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="aaca8-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true,
      "region": "region-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectorGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

