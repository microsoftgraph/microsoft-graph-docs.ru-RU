---
title: Список memberOf
description: Извлечение соединитекторной группы, членом в который является соедините.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 4a069e0e501d1916b310daa390a2b2af0de5318f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047218"
---
# <a name="list-memberof"></a><span data-ttu-id="dee43-103">Список memberOf</span><span class="sxs-lookup"><span data-stu-id="dee43-103">List memberOf</span></span>

<span data-ttu-id="dee43-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dee43-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dee43-105">[Извлечение соединителиГрупп](../resources/connectorgroup.md) [соединитетеля](../resources/connector.md) является членом.</span><span class="sxs-lookup"><span data-stu-id="dee43-105">Retrieve the [connectorGroup](../resources/connectorgroup.md) the [connector](../resources/connector.md) is a member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="dee43-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="dee43-106">Permissions</span></span>
<span data-ttu-id="dee43-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="dee43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dee43-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="dee43-109">Permission type</span></span>      | <span data-ttu-id="dee43-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="dee43-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dee43-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="dee43-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dee43-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dee43-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dee43-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="dee43-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dee43-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dee43-114">Not supported.</span></span>    |
|<span data-ttu-id="dee43-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="dee43-115">Application</span></span> | <span data-ttu-id="dee43-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dee43-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="dee43-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="dee43-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dee43-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="dee43-118">Optional query parameters</span></span>
<span data-ttu-id="dee43-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="dee43-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dee43-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="dee43-120">Request headers</span></span>
| <span data-ttu-id="dee43-121">Имя</span><span class="sxs-lookup"><span data-stu-id="dee43-121">Name</span></span>      |<span data-ttu-id="dee43-122">Описание</span><span class="sxs-lookup"><span data-stu-id="dee43-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dee43-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dee43-123">Authorization</span></span>  | <span data-ttu-id="dee43-124">Носителер.</span><span class="sxs-lookup"><span data-stu-id="dee43-124">Bearer.</span></span> <span data-ttu-id="dee43-125">Обязательна</span><span class="sxs-lookup"><span data-stu-id="dee43-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="dee43-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="dee43-126">Request body</span></span>
<span data-ttu-id="dee43-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="dee43-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dee43-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="dee43-128">Response</span></span>

<span data-ttu-id="dee43-129">В случае успешной работы этот метод возвращает код отклика и коллекцию объектов `200 OK` [connectorGroup](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="dee43-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dee43-130">Пример</span><span class="sxs-lookup"><span data-stu-id="dee43-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dee43-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="dee43-131">Request</span></span>
<span data-ttu-id="dee43-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="dee43-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dee43-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dee43-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "connector_get_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="dee43-134">C#</span><span class="sxs-lookup"><span data-stu-id="dee43-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/connector-get-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dee43-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dee43-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/connector-get-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dee43-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dee43-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/connector-get-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dee43-137">Java</span><span class="sxs-lookup"><span data-stu-id="dee43-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/connector-get-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dee43-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="dee43-138">Response</span></span>
<span data-ttu-id="dee43-139">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="dee43-139">The following is an example of the response.</span></span> <span data-ttu-id="dee43-140">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="dee43-140">Note: The response object shown here might be shortened for readability.</span></span>
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
      "isDefault": false,
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

