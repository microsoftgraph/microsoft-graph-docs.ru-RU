---
title: Создание дела
description: Используйте этот API для создания нового случая.
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 69a099cf250036f86e6481a818b4dbdc581c7aea
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/13/2021
ms.locfileid: "50773734"
---
# <a name="create-case"></a><span data-ttu-id="c3e16-103">Создание дела</span><span class="sxs-lookup"><span data-stu-id="c3e16-103">Create case</span></span>

<span data-ttu-id="c3e16-104">Пространство имен: microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="c3e16-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3e16-105">Создайте новый [объект case.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="c3e16-105">Create a new [case](../resources/ediscovery-case.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c3e16-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e16-106">Permissions</span></span>

<span data-ttu-id="c3e16-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3e16-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3e16-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c3e16-109">Permission type</span></span>|<span data-ttu-id="c3e16-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c3e16-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3e16-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c3e16-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c3e16-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3e16-112">eDiscovery.Read.All, eDiscovery.ReadWrite.All</span></span>|
|<span data-ttu-id="c3e16-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c3e16-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3e16-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e16-114">Not supported.</span></span>|
|<span data-ttu-id="c3e16-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c3e16-115">Application</span></span>|<span data-ttu-id="c3e16-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c3e16-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3e16-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c3e16-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /compliance/ediscovery/cases
```

## <a name="request-headers"></a><span data-ttu-id="c3e16-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c3e16-118">Request headers</span></span>

| <span data-ttu-id="c3e16-119">Имя</span><span class="sxs-lookup"><span data-stu-id="c3e16-119">Name</span></span>          | <span data-ttu-id="c3e16-120">Описание</span><span class="sxs-lookup"><span data-stu-id="c3e16-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c3e16-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c3e16-121">Authorization</span></span> | <span data-ttu-id="c3e16-p102">Bearer {токен}. Обязательный.</span><span class="sxs-lookup"><span data-stu-id="c3e16-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3e16-124">Текст запроса</span><span class="sxs-lookup"><span data-stu-id="c3e16-124">Request body</span></span>

<span data-ttu-id="c3e16-125">В теле запроса поставляем представление JSON объекта [дела.](../resources/ediscovery-case.md)</span><span class="sxs-lookup"><span data-stu-id="c3e16-125">In the request body, supply a JSON representation of a [case](../resources/ediscovery-case.md) object.</span></span> <span data-ttu-id="c3e16-126">В следующей таблице перечислены свойства, которые можно представить с помощью вызова.</span><span class="sxs-lookup"><span data-stu-id="c3e16-126">The following table lists properties that can be submitted with the call.</span></span>

| <span data-ttu-id="c3e16-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3e16-127">Property</span></span>     | <span data-ttu-id="c3e16-128">Тип</span><span class="sxs-lookup"><span data-stu-id="c3e16-128">Type</span></span>        | <span data-ttu-id="c3e16-129">Описание</span><span class="sxs-lookup"><span data-stu-id="c3e16-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="c3e16-130">displayName</span><span class="sxs-lookup"><span data-stu-id="c3e16-130">displayName</span></span>  | <span data-ttu-id="c3e16-131">string</span><span class="sxs-lookup"><span data-stu-id="c3e16-131">string</span></span>      | <span data-ttu-id="c3e16-132">Имя дела об обнаружении электронной почты.</span><span class="sxs-lookup"><span data-stu-id="c3e16-132">The name of the eDiscovery case.</span></span> |

## <a name="response"></a><span data-ttu-id="c3e16-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3e16-133">Response</span></span>

<span data-ttu-id="c3e16-134">В случае успеха этот метод возвращает код отклика и новый `201 Created` [объект microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="c3e16-134">If successful, this method returns a `201 Created` response code and a new [microsoft.graph.ediscovery.case](../resources/ediscovery-case.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c3e16-135">Примеры</span><span class="sxs-lookup"><span data-stu-id="c3e16-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c3e16-136">Запрос</span><span class="sxs-lookup"><span data-stu-id="c3e16-136">Request</span></span>

<span data-ttu-id="c3e16-137">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c3e16-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c3e16-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="c3e16-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "post_case"
}-->

```http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases
Content-type: application/json

{
    "displayName": "My Case 1",
}
```

# <a name="c"></a>[<span data-ttu-id="c3e16-139">C#</span><span class="sxs-lookup"><span data-stu-id="c3e16-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/post-case-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c3e16-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c3e16-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/post-case-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c3e16-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c3e16-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/post-case-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c3e16-142">Java</span><span class="sxs-lookup"><span data-stu-id="c3e16-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/post-case-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c3e16-143">Отклик</span><span class="sxs-lookup"><span data-stu-id="c3e16-143">Response</span></span>

<span data-ttu-id="c3e16-144">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c3e16-144">The following is an example of the response.</span></span>

> <span data-ttu-id="c3e16-p104">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c3e16-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.ediscovery.case"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/compliance/ediscovery/$metadata#cases/$entity",
    "id": "061b9a92-8926-4bd9-b41d-abf35edc7583",
    "displayName": "My Case 1",
    "description": "",
    "createdBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "createdDateTime": "2020-02-20T22:42:28.5505500Z",
    "lastModifiedBy": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "eDiscovery admin"
        }
    },
    "lastModifiedDateTime": "2020-02-20T22:42:28.5505500Z",
    "status": "active",
    "closedBy": null,
    "closedDateTime": null,
    "externalId": ""
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create case",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
