---
title: Получение connectorGroup
description: Извлечение свойств объекта connectorGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 8052f4aaf16ee16f89141c2715d519360e33dead
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129601"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="05ae3-103">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="05ae3-103">Get connectorGroup</span></span>

<span data-ttu-id="05ae3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="05ae3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05ae3-105">Извлечение свойств [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="05ae3-105">Retrieve the properties of a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="05ae3-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="05ae3-106">Permissions</span></span>
<span data-ttu-id="05ae3-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="05ae3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05ae3-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="05ae3-109">Permission type</span></span>      | <span data-ttu-id="05ae3-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="05ae3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05ae3-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="05ae3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="05ae3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="05ae3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="05ae3-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="05ae3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05ae3-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05ae3-114">Not supported.</span></span>    |
|<span data-ttu-id="05ae3-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="05ae3-115">Application</span></span> | <span data-ttu-id="05ae3-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="05ae3-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="05ae3-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="05ae3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="05ae3-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="05ae3-118">Optional query parameters</span></span>
<span data-ttu-id="05ae3-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="05ae3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="05ae3-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="05ae3-120">Request headers</span></span>
| <span data-ttu-id="05ae3-121">Имя</span><span class="sxs-lookup"><span data-stu-id="05ae3-121">Name</span></span>      |<span data-ttu-id="05ae3-122">Описание</span><span class="sxs-lookup"><span data-stu-id="05ae3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="05ae3-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="05ae3-123">Authorization</span></span>  | <span data-ttu-id="05ae3-124">Bearer.</span><span class="sxs-lookup"><span data-stu-id="05ae3-124">Bearer.</span></span> <span data-ttu-id="05ae3-125">Обязательна</span><span class="sxs-lookup"><span data-stu-id="05ae3-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="05ae3-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="05ae3-126">Request body</span></span>
<span data-ttu-id="05ae3-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="05ae3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05ae3-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="05ae3-128">Response</span></span>

<span data-ttu-id="05ae3-129">В случае успеха этот метод возвращает код отклика и объект `200 OK` [connectorGroup](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="05ae3-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05ae3-130">Пример</span><span class="sxs-lookup"><span data-stu-id="05ae3-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="05ae3-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="05ae3-131">Request</span></span>
<span data-ttu-id="05ae3-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="05ae3-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="05ae3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="05ae3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="05ae3-134">C#</span><span class="sxs-lookup"><span data-stu-id="05ae3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="05ae3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="05ae3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="05ae3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05ae3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="05ae3-137">Java</span><span class="sxs-lookup"><span data-stu-id="05ae3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="05ae3-138">Отклик</span><span class="sxs-lookup"><span data-stu-id="05ae3-138">Response</span></span>
<span data-ttu-id="05ae3-139">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="05ae3-139">The following is an example of the response.</span></span> <span data-ttu-id="05ae3-140">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="05ae3-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="05ae3-141">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="05ae3-141">All of the properties will be returned from an actual call.</span></span>
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

