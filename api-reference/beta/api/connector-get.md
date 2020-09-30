---
title: Получение соединителя
description: Получение свойств объекта Connector.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 69f4a164a6dd43273d67bd6c43e175922a81626a
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/30/2020
ms.locfileid: "48312129"
---
# <a name="get-connector"></a><span data-ttu-id="acd96-103">Получение соединителя</span><span class="sxs-lookup"><span data-stu-id="acd96-103">Get connector</span></span>

<span data-ttu-id="acd96-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="acd96-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="acd96-105">Получение свойств и связей объекта [Connector](../resources/connector.md) .</span><span class="sxs-lookup"><span data-stu-id="acd96-105">Retrieve the properties and relationships of a [connector](../resources/connector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="acd96-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="acd96-106">Permissions</span></span>
<span data-ttu-id="acd96-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="acd96-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="acd96-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="acd96-109">Permission type</span></span>      | <span data-ttu-id="acd96-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="acd96-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="acd96-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="acd96-111">Delegated (work or school account)</span></span> | <span data-ttu-id="acd96-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="acd96-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="acd96-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="acd96-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="acd96-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd96-114">Not supported.</span></span>    |
|<span data-ttu-id="acd96-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="acd96-115">Application</span></span> | <span data-ttu-id="acd96-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="acd96-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="acd96-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="acd96-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="acd96-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="acd96-118">Optional query parameters</span></span>
<span data-ttu-id="acd96-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="acd96-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="acd96-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="acd96-120">Request headers</span></span>
| <span data-ttu-id="acd96-121">Имя</span><span class="sxs-lookup"><span data-stu-id="acd96-121">Name</span></span>      |<span data-ttu-id="acd96-122">Описание</span><span class="sxs-lookup"><span data-stu-id="acd96-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="acd96-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="acd96-123">Authorization</span></span>  | <span data-ttu-id="acd96-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="acd96-124">Bearer.</span></span> <span data-ttu-id="acd96-125">Обязательный</span><span class="sxs-lookup"><span data-stu-id="acd96-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="acd96-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="acd96-126">Request body</span></span>
<span data-ttu-id="acd96-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="acd96-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="acd96-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="acd96-128">Response</span></span>

<span data-ttu-id="acd96-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="acd96-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="acd96-130">Пример</span><span class="sxs-lookup"><span data-stu-id="acd96-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="acd96-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="acd96-131">Request</span></span>

<span data-ttu-id="acd96-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="acd96-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="acd96-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="acd96-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="acd96-134">C#</span><span class="sxs-lookup"><span data-stu-id="acd96-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="acd96-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="acd96-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="acd96-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="acd96-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="acd96-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="acd96-137">Response</span></span>
<span data-ttu-id="acd96-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="acd96-138">The following is an example of the response.</span></span> <span data-ttu-id="acd96-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="acd96-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="acd96-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="acd96-140">All of the properties will be returned from an actual call.</span></span>
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