---
title: Создание connectorGroup
description: Используйте этот API для создания нового соединитетеляGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: dd11c3b86bc2e4036f56b3bd5d83f426fab0e1bd
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047156"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="4a40f-103">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="4a40f-103">Create connectorGroup</span></span>

<span data-ttu-id="4a40f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a40f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a40f-105">Создайте [новый соединитекторGroup](../resources/connectorgroup.md).</span><span class="sxs-lookup"><span data-stu-id="4a40f-105">Create a new [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a40f-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a40f-106">Permissions</span></span>
<span data-ttu-id="4a40f-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a40f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a40f-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a40f-109">Permission type</span></span>      | <span data-ttu-id="4a40f-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a40f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a40f-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a40f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a40f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4a40f-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4a40f-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a40f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a40f-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a40f-114">Not supported.</span></span>    |
|<span data-ttu-id="4a40f-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a40f-115">Application</span></span> | <span data-ttu-id="4a40f-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a40f-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4a40f-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a40f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="4a40f-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="4a40f-118">Request headers</span></span>
| <span data-ttu-id="4a40f-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4a40f-119">Name</span></span>       | <span data-ttu-id="4a40f-120">Описание</span><span class="sxs-lookup"><span data-stu-id="4a40f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="4a40f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a40f-121">Authorization</span></span>  | <span data-ttu-id="4a40f-122">Носителер.</span><span class="sxs-lookup"><span data-stu-id="4a40f-122">Bearer.</span></span> <span data-ttu-id="4a40f-123">Requried</span><span class="sxs-lookup"><span data-stu-id="4a40f-123">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a40f-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a40f-124">Request body</span></span>
<span data-ttu-id="4a40f-125">В теле запроса поставляем представление JSON объекта [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="4a40f-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4a40f-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a40f-126">Response</span></span>

<span data-ttu-id="4a40f-127">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект connectorGroup](../resources/connectorgroup.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="4a40f-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a40f-128">Пример</span><span class="sxs-lookup"><span data-stu-id="4a40f-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4a40f-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a40f-129">Request</span></span>
<span data-ttu-id="4a40f-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a40f-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a40f-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a40f-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "isDefault": false
}
```
# <a name="c"></a>[<span data-ttu-id="4a40f-132">C#</span><span class="sxs-lookup"><span data-stu-id="4a40f-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectorgroup-from-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a40f-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a40f-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a40f-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a40f-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectorgroup-from-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a40f-135">Java</span><span class="sxs-lookup"><span data-stu-id="4a40f-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectorgroup-from-connectorgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="4a40f-136">В теле запроса поставляем представление JSON объекта [connectorGroup.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="4a40f-136">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="4a40f-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a40f-137">Response</span></span>
<span data-ttu-id="4a40f-138">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a40f-138">Here is an example of the response.</span></span> <span data-ttu-id="4a40f-139">Примечание. Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a40f-139">Note: The response object shown here might be shortened for readability.</span></span>
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



