---
title: Добавление соединителя в Коннекторграуп
description: Используйте этот API, чтобы добавить соединитель для нового Коннекторграуп.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 00f2ada7d46831b6b0bfbae0db4174e3ca2e9c90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009081"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="85454-103">Добавление соединителя для connectorGroup</span><span class="sxs-lookup"><span data-stu-id="85454-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="85454-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85454-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85454-105">Добавление [соединителя](../resources/connector.md)  в [коннекторграуп](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="85454-105">Add a [connector](../resources/connector.md)  to a [connectorGroup](../resources/connectorgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="85454-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="85454-106">Permissions</span></span>
<span data-ttu-id="85454-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="85454-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="85454-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="85454-109">Permission type</span></span>      | <span data-ttu-id="85454-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="85454-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="85454-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="85454-111">Delegated (work or school account)</span></span> | <span data-ttu-id="85454-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="85454-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="85454-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="85454-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="85454-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85454-114">Not supported.</span></span>    |
|<span data-ttu-id="85454-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="85454-115">Application</span></span> | <span data-ttu-id="85454-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="85454-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="85454-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="85454-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref

```
## <a name="request-headers"></a><span data-ttu-id="85454-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="85454-118">Request headers</span></span>
| <span data-ttu-id="85454-119">Имя</span><span class="sxs-lookup"><span data-stu-id="85454-119">Name</span></span>       | <span data-ttu-id="85454-120">Описание</span><span class="sxs-lookup"><span data-stu-id="85454-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="85454-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="85454-121">Authorization</span></span>  | <span data-ttu-id="85454-122">Носителя.</span><span class="sxs-lookup"><span data-stu-id="85454-122">Bearer.</span></span> <span data-ttu-id="85454-123">Обязательно</span><span class="sxs-lookup"><span data-stu-id="85454-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="85454-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="85454-124">Request body</span></span>
<span data-ttu-id="85454-125">В тексте запроса добавьте представление объекта [коннекторграуп](../resources/connectorgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85454-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="85454-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="85454-126">Response</span></span>

<span data-ttu-id="85454-127">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [коннекторграуп](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="85454-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="85454-128">Пример</span><span class="sxs-lookup"><span data-stu-id="85454-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="85454-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="85454-129">Request</span></span>
<span data-ttu-id="85454-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="85454-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="85454-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="85454-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="85454-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="85454-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="85454-133">В тексте запроса добавьте представление объекта [коннекторграуп](../resources/connectorgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="85454-133">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="85454-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="85454-134">Response</span></span>
<span data-ttu-id="85454-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="85454-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


