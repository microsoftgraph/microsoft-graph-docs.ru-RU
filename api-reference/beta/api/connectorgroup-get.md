---
title: Получение connectorGroup
description: Получение свойств объекта Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 62e6585c32993f5fa14905ce76e4830439ab1c7e
ms.sourcegitcommit: c20276369a8834a259f24038e7ee5c33de02660b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2020
ms.locfileid: "48371742"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="e430a-103">Получение connectorGroup</span><span class="sxs-lookup"><span data-stu-id="e430a-103">Get connectorGroup</span></span>

<span data-ttu-id="e430a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e430a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e430a-105">Получение свойств объекта [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="e430a-105">Retrieve the properties of a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e430a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="e430a-106">Permissions</span></span>
<span data-ttu-id="e430a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e430a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e430a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="e430a-109">Permission type</span></span>      | <span data-ttu-id="e430a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="e430a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e430a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="e430a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e430a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e430a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e430a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="e430a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e430a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e430a-114">Not supported.</span></span>    |
|<span data-ttu-id="e430a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="e430a-115">Application</span></span> | <span data-ttu-id="e430a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e430a-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="e430a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="e430a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e430a-118">Необязательные параметры запросов</span><span class="sxs-lookup"><span data-stu-id="e430a-118">Optional query parameters</span></span>
<span data-ttu-id="e430a-119">Этот метод поддерживает [параметры запросов OData](/graph/query-parameters) для настройки ответа.</span><span class="sxs-lookup"><span data-stu-id="e430a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e430a-120">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="e430a-120">Request headers</span></span>
| <span data-ttu-id="e430a-121">Имя</span><span class="sxs-lookup"><span data-stu-id="e430a-121">Name</span></span>      |<span data-ttu-id="e430a-122">Описание</span><span class="sxs-lookup"><span data-stu-id="e430a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e430a-123">Авторизация</span><span class="sxs-lookup"><span data-stu-id="e430a-123">Authorization</span></span>  | <span data-ttu-id="e430a-124">Носителя.</span><span class="sxs-lookup"><span data-stu-id="e430a-124">Bearer.</span></span> <span data-ttu-id="e430a-125">Обязательно</span><span class="sxs-lookup"><span data-stu-id="e430a-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e430a-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="e430a-126">Request body</span></span>
<span data-ttu-id="e430a-127">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="e430a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e430a-128">Отклик</span><span class="sxs-lookup"><span data-stu-id="e430a-128">Response</span></span>

<span data-ttu-id="e430a-129">В случае успешного выполнения этот метод возвращает `200 OK` код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="e430a-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e430a-130">Пример</span><span class="sxs-lookup"><span data-stu-id="e430a-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e430a-131">Запрос</span><span class="sxs-lookup"><span data-stu-id="e430a-131">Request</span></span>
<span data-ttu-id="e430a-132">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="e430a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e430a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e430a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="e430a-134">C#</span><span class="sxs-lookup"><span data-stu-id="e430a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e430a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e430a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e430a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e430a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e430a-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="e430a-137">Response</span></span>
<span data-ttu-id="e430a-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="e430a-138">The following is an example of the response.</span></span> <span data-ttu-id="e430a-139">Примечание. Представленный здесь объект отклика может быть усечен для краткости.</span><span class="sxs-lookup"><span data-stu-id="e430a-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e430a-140">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="e430a-140">All of the properties will be returned from an actual call.</span></span>
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
