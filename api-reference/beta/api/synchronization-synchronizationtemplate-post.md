---
title: Создание Синчронизатионтемплате
description: Создайте новый шаблон синхронизации для конкретного приложения.
localization_priority: Normal
doc_type: apiPageType
author: ArvindHarinder1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b75d5e2f052983cab54fe1cdfd557e03b7778e6e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471140"
---
# <a name="create-synchronizationtemplate"></a><span data-ttu-id="29dcd-103">Создание Синчронизатионтемплате</span><span class="sxs-lookup"><span data-stu-id="29dcd-103">Create synchronizationTemplate</span></span>

<span data-ttu-id="29dcd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29dcd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29dcd-105">Создайте новый шаблон синхронизации для конкретного приложения.</span><span class="sxs-lookup"><span data-stu-id="29dcd-105">Create a new synchronization template for a given application.</span></span>

## <a name="permissions"></a><span data-ttu-id="29dcd-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="29dcd-106">Permissions</span></span>
<span data-ttu-id="29dcd-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="29dcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29dcd-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="29dcd-109">Permission type</span></span>                        | <span data-ttu-id="29dcd-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="29dcd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="29dcd-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="29dcd-111">Delegated (work or school account)</span></span>     |<span data-ttu-id="29dcd-112">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29dcd-112">Directory.ReadWrite.All</span></span>  |
|<span data-ttu-id="29dcd-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="29dcd-113">Delegated (personal Microsoft account)</span></span> |<span data-ttu-id="29dcd-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29dcd-114">Not supported.</span></span>|
|<span data-ttu-id="29dcd-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="29dcd-115">Application</span></span>                            |<span data-ttu-id="29dcd-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="29dcd-116">Not supported.</span></span>| 

### <a name="http-request"></a><span data-ttu-id="29dcd-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="29dcd-117">HTTP Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/synchronization/templates/
```

## <a name="request-headers"></a><span data-ttu-id="29dcd-118">Заголовки запроса</span><span class="sxs-lookup"><span data-stu-id="29dcd-118">Request headers</span></span>

| <span data-ttu-id="29dcd-119">Имя</span><span class="sxs-lookup"><span data-stu-id="29dcd-119">Name</span></span>           | <span data-ttu-id="29dcd-120">Тип</span><span class="sxs-lookup"><span data-stu-id="29dcd-120">Type</span></span>    | <span data-ttu-id="29dcd-121">Описание</span><span class="sxs-lookup"><span data-stu-id="29dcd-121">Description</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="29dcd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="29dcd-122">Authorization</span></span>  | <span data-ttu-id="29dcd-123">string</span><span class="sxs-lookup"><span data-stu-id="29dcd-123">string</span></span>  | <span data-ttu-id="29dcd-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="29dcd-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="29dcd-126">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="29dcd-126">Request body</span></span>

<span data-ttu-id="29dcd-127">В теле запроса добавьте объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) , который требуется создать.</span><span class="sxs-lookup"><span data-stu-id="29dcd-127">In the request body, supply the [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object to be created.</span></span> <span data-ttu-id="29dcd-128">`id`Свойства `applicationId` и `factoryTag` свойства являются обязательными.</span><span class="sxs-lookup"><span data-stu-id="29dcd-128">The `id`, `applicationId` and `factoryTag` properties are required.</span></span> <span data-ttu-id="29dcd-129">Если с `schema` шаблоном не предоставляется никакой шаблон, будет использоваться схема по умолчанию, связанная со `factoryTag` свойством.</span><span class="sxs-lookup"><span data-stu-id="29dcd-129">When no `schema` is provided with the template, the default schema associated with the `factoryTag` property will be used.</span></span>

### <a name="response"></a><span data-ttu-id="29dcd-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="29dcd-130">Response</span></span>

<span data-ttu-id="29dcd-131">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [синчронизатионтемплате](../resources/synchronization-synchronizationtemplate.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="29dcd-131">If successful, this method returns a `201 Created` response code and a [synchronizationTemplate](../resources/synchronization-synchronizationtemplate.md) object in the response body.</span></span>

### <a name="example"></a><span data-ttu-id="29dcd-132">Пример</span><span class="sxs-lookup"><span data-stu-id="29dcd-132">Example</span></span>

##### <a name="request"></a><span data-ttu-id="29dcd-133">Запрос</span><span class="sxs-lookup"><span data-stu-id="29dcd-133">Request</span></span>
<span data-ttu-id="29dcd-134">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="29dcd-134">The following is an example of a request.</span></span>

# <a name="http"></a>[<span data-ttu-id="29dcd-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="29dcd-135">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="29dcd-136">C#</span><span class="sxs-lookup"><span data-stu-id="29dcd-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-synchronizationtemplate-from-synchronization-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29dcd-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29dcd-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-synchronizationtemplate-from-synchronization-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29dcd-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29dcd-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-synchronizationtemplate-from-synchronization-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="29dcd-139">Отклик</span><span class="sxs-lookup"><span data-stu-id="29dcd-139">Response</span></span>
<span data-ttu-id="29dcd-140">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="29dcd-140">The following is an example of a response.</span></span>
><span data-ttu-id="29dcd-141">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="29dcd-141">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="29dcd-142">При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="29dcd-142">All the properties will be returned in an actual call.</span></span>
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
