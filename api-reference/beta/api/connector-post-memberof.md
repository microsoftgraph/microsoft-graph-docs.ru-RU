---
title: Добавление соединителю в connectorGroup
description: Этот API используется для добавления соединителю в новый connectorGroup.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 39822b0415c8c52944f89d86adc74d38af981020
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753011"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="1b0ac-103">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="1b0ac-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="1b0ac-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b0ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b0ac-105">Добавление [соединителю](../resources/connector.md) в [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="1b0ac-105">Add a [connector](../resources/connector.md)  to a [connectorGroup](../resources/connectorgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="1b0ac-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="1b0ac-106">Permissions</span></span>
<span data-ttu-id="1b0ac-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1b0ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b0ac-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="1b0ac-109">Permission type</span></span>      | <span data-ttu-id="1b0ac-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="1b0ac-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b0ac-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="1b0ac-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1b0ac-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1b0ac-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1b0ac-113">Делегированное (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="1b0ac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b0ac-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0ac-114">Not supported.</span></span>    |
|<span data-ttu-id="1b0ac-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="1b0ac-115">Application</span></span> | <span data-ttu-id="1b0ac-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b0ac-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="1b0ac-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="1b0ac-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref

```
## <a name="request-headers"></a><span data-ttu-id="1b0ac-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1b0ac-118">Request headers</span></span>
| <span data-ttu-id="1b0ac-119">Имя</span><span class="sxs-lookup"><span data-stu-id="1b0ac-119">Name</span></span>       | <span data-ttu-id="1b0ac-120">Описание</span><span class="sxs-lookup"><span data-stu-id="1b0ac-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1b0ac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b0ac-121">Authorization</span></span>  | <span data-ttu-id="1b0ac-122">Bearer.</span><span class="sxs-lookup"><span data-stu-id="1b0ac-122">Bearer.</span></span> <span data-ttu-id="1b0ac-123">Обязательна</span><span class="sxs-lookup"><span data-stu-id="1b0ac-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b0ac-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="1b0ac-124">Request body</span></span>
<span data-ttu-id="1b0ac-125">В теле запроса укажет представление объекта [connectorGroup](../resources/connectorgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1b0ac-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1b0ac-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b0ac-126">Response</span></span>

<span data-ttu-id="1b0ac-127">В случае успеха этот метод возвращает код отклика и `201 Created` [объект connectorGroup](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="1b0ac-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b0ac-128">Пример</span><span class="sxs-lookup"><span data-stu-id="1b0ac-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1b0ac-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="1b0ac-129">Request</span></span>
<span data-ttu-id="1b0ac-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="1b0ac-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1b0ac-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="1b0ac-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connector"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref
Content-type: application/json
Content-length: 99

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="1b0ac-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1b0ac-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="1b0ac-133">C#</span><span class="sxs-lookup"><span data-stu-id="1b0ac-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectorgroup-from-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1b0ac-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1b0ac-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectorgroup-from-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1b0ac-135">Java</span><span class="sxs-lookup"><span data-stu-id="1b0ac-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectorgroup-from-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1b0ac-136">В теле запроса укажете представление объекта [connectorGroup](../resources/connectorgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="1b0ac-136">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1b0ac-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="1b0ac-137">Response</span></span>
<span data-ttu-id="1b0ac-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="1b0ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


