---
title: Добавление соединителя в Коннекторграуп
description: Используйте этот API, чтобы добавить соединитель в Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4b147b384223bee7bc7eb245b11e19c5600d0fed
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681192"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="0af36-103">Добавление соединителя в Коннекторграуп</span><span class="sxs-lookup"><span data-stu-id="0af36-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="0af36-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0af36-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0af36-105">Добавление [соединителя](../resources/connector.md) в [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="0af36-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="0af36-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0af36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af36-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="0af36-108">Permission type</span></span>      | <span data-ttu-id="0af36-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="0af36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0af36-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="0af36-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0af36-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0af36-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0af36-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="0af36-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0af36-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0af36-113">Not supported.</span></span>    |
|<span data-ttu-id="0af36-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="0af36-114">Application</span></span> | <span data-ttu-id="0af36-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0af36-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0af36-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="0af36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="0af36-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="0af36-117">Request headers</span></span>
| <span data-ttu-id="0af36-118">Имя</span><span class="sxs-lookup"><span data-stu-id="0af36-118">Name</span></span>       | <span data-ttu-id="0af36-119">Описание</span><span class="sxs-lookup"><span data-stu-id="0af36-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0af36-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af36-120">Authorization</span></span>  | <span data-ttu-id="0af36-121">Носителя.</span><span class="sxs-lookup"><span data-stu-id="0af36-121">Bearer.</span></span> <span data-ttu-id="0af36-122">Обязательное</span><span class="sxs-lookup"><span data-stu-id="0af36-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="0af36-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="0af36-123">Request body</span></span>
<span data-ttu-id="0af36-124">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0af36-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0af36-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="0af36-125">Response</span></span>

<span data-ttu-id="0af36-126">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [Connector](../resources/connector.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="0af36-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0af36-127">Пример</span><span class="sxs-lookup"><span data-stu-id="0af36-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0af36-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="0af36-128">Request</span></span>
<span data-ttu-id="0af36-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="0af36-129">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0af36-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="0af36-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="0af36-131">C#</span><span class="sxs-lookup"><span data-stu-id="0af36-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connector-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0af36-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0af36-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connector-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0af36-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0af36-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connector-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="0af36-134">В тексте запроса добавьте представление ссылки на объект [Connector](../resources/connector.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0af36-134">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0af36-135">Отклик</span><span class="sxs-lookup"><span data-stu-id="0af36-135">Response</span></span>
<span data-ttu-id="0af36-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="0af36-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
