---
title: Создание connectorGroup
description: Используйте этот API для создания соединителиGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 07adf13a703868eb1ec77bf67325d6a8eef45ebf
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50129984"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="f4b86-103">Создание connectorGroup</span><span class="sxs-lookup"><span data-stu-id="f4b86-103">Create connectorGroup</span></span>

<span data-ttu-id="f4b86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f4b86-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4b86-105">Создание [соединителиГруппы.](../resources/connectorgroup.md)</span><span class="sxs-lookup"><span data-stu-id="f4b86-105">Create a new [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f4b86-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="f4b86-106">Permissions</span></span>
<span data-ttu-id="f4b86-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4b86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4b86-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="f4b86-109">Permission type</span></span>      | <span data-ttu-id="f4b86-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="f4b86-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f4b86-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="f4b86-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f4b86-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f4b86-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f4b86-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="f4b86-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f4b86-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f4b86-114">Not supported.</span></span>    |
|<span data-ttu-id="f4b86-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="f4b86-115">Application</span></span> | <span data-ttu-id="f4b86-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4b86-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f4b86-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="f4b86-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="f4b86-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="f4b86-118">Request headers</span></span>
| <span data-ttu-id="f4b86-119">Имя</span><span class="sxs-lookup"><span data-stu-id="f4b86-119">Name</span></span>       | <span data-ttu-id="f4b86-120">Описание</span><span class="sxs-lookup"><span data-stu-id="f4b86-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f4b86-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="f4b86-121">Authorization</span></span>  | <span data-ttu-id="f4b86-122">Bearer.</span><span class="sxs-lookup"><span data-stu-id="f4b86-122">Bearer.</span></span> <span data-ttu-id="f4b86-123">Requried</span><span class="sxs-lookup"><span data-stu-id="f4b86-123">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4b86-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="f4b86-124">Request body</span></span>
<span data-ttu-id="f4b86-125">В теле запроса укажете представление объекта [connectorGroup](../resources/connectorgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="f4b86-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="f4b86-126">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4b86-126">Response</span></span>

<span data-ttu-id="f4b86-127">В случае успеха этот метод возвращает код отклика и `201 Created` [объект connectorGroup](../resources/connectorgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="f4b86-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4b86-128">Пример</span><span class="sxs-lookup"><span data-stu-id="f4b86-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f4b86-129">Запрос</span><span class="sxs-lookup"><span data-stu-id="f4b86-129">Request</span></span>
<span data-ttu-id="f4b86-130">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="f4b86-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f4b86-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4b86-131">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f4b86-132">C#</span><span class="sxs-lookup"><span data-stu-id="f4b86-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectorgroup-from-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4b86-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4b86-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4b86-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4b86-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectorgroup-from-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4b86-135">Java</span><span class="sxs-lookup"><span data-stu-id="f4b86-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectorgroup-from-connectorgroups-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="f4b86-136">В теле запроса укажете представление объекта [connectorGroup](../resources/connectorgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="f4b86-136">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f4b86-137">Отклик</span><span class="sxs-lookup"><span data-stu-id="f4b86-137">Response</span></span>
<span data-ttu-id="f4b86-p103">Ниже приведен пример отклика. Примечание. Объект отклика, показанный здесь, может быть усечен для краткости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="f4b86-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



