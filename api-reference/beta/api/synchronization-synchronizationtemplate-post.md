---
title: Создание synchronizationTemplate
description: Создайте новый шаблон синхронизации для заданного приложения.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: applications
ms.openlocfilehash: 054e5dfc672f3336e5c8d633e05c1db82e350fdd
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137244"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="4a961-103">Создание synchronizationTemplate</span><span class="sxs-lookup"><span data-stu-id="4a961-103">Create synchronizationTemplate</span></span>

<span data-ttu-id="4a961-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a961-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a961-105">Создайте новый шаблон синхронизации для заданного приложения.</span><span class="sxs-lookup"><span data-stu-id="4a961-105">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="4a961-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="4a961-106">Permissions</span></span>
<span data-ttu-id="4a961-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4a961-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4a961-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="4a961-109">Permission type</span></span>                        | <span data-ttu-id="4a961-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="4a961-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a961-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="4a961-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="4a961-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a961-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="4a961-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="4a961-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="4a961-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a961-114">Not supported.</span></span>|
|<span data-ttu-id="4a961-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="4a961-115">Application</span></span>                            |<span data-ttu-id="4a961-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4a961-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="4a961-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="4a961-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="4a961-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="4a961-118">Request headers</span></span>

| <span data-ttu-id="4a961-119">Имя</span><span class="sxs-lookup"><span data-stu-id="4a961-119">Name</span></span>           | <span data-ttu-id="4a961-120">Тип</span><span class="sxs-lookup"><span data-stu-id="4a961-120">Type</span></span>    | <span data-ttu-id="4a961-121">Описание</span><span class="sxs-lookup"><span data-stu-id="4a961-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="4a961-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a961-122">Authorization</span></span>  | <span data-ttu-id="4a961-123">string</span><span class="sxs-lookup"><span data-stu-id="4a961-123">string</span></span>  | <span data-ttu-id="4a961-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="4a961-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4a961-126">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="4a961-126">Request body</span></span>

<span data-ttu-id="4a961-127">В теле запроса укажи объект [synchronizationTemplate,](../resources/synchronization-synchronizationtemplate.md) который необходимо создать.</span><span class="sxs-lookup"><span data-stu-id="4a961-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="4a961-128">Свойства и `id` свойства `applicationId` являются `factoryTag` обязательной.</span><span class="sxs-lookup"><span data-stu-id="4a961-128">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="4a961-129">Если шаблон не предоставляется, будет использоваться схема по умолчанию, связанная `schema` со `factoryTag` свойством.</span><span class="sxs-lookup"><span data-stu-id="4a961-129">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="4a961-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a961-130">Response</span></span>

<span data-ttu-id="4a961-131">В случае успеха этот метод возвращает код отклика и объект `201 Created` [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="4a961-131">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="4a961-132">Пример</span><span class="sxs-lookup"><span data-stu-id="4a961-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4a961-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="4a961-133">Request</span></span>
<span data-ttu-id="4a961-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="4a961-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a961-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a961-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_synchronizationtemplate_from_synchronization"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/synchronization/templates
Content-type: application/json

{ 
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM"
}
```
# <a name="c"></a>[<span data-ttu-id="4a961-136">C#</span><span class="sxs-lookup"><span data-stu-id="4a961-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4a961-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a961-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a961-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a961-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a961-139">Java</span><span class="sxs-lookup"><span data-stu-id="4a961-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-synchronizationtemplate-from-synchronization-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4a961-140">Отклик</span><span class="sxs-lookup"><span data-stu-id="4a961-140">Response</span></span>
<span data-ttu-id="4a961-141">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="4a961-141">The following is an example of a response.</span></span>
><span data-ttu-id="4a961-142">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="4a961-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="4a961-143">Все свойства будут возвращены при фактическом вызове.</span><span class="sxs-lookup"><span data-stu-id="4a961-143">All the properties will be returned in an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.synchronizationTemplate"
} -->
```http
HTTP/1.1 201 Created

{
    "id": "SCIM-Test1",
    "applicationId": "{id}",
    "factoryTag": "CustomSCIM",
    "schema": {
        "directories": [],
        "synchronizationRules": []
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create synchronizationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


