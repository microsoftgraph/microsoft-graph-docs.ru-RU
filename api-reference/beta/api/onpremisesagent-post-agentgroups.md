---
title: Назначение Онпремисесажент для Онпремисесажентграуп
description: Назначьте Онпремисесажент для Онпремисесажентграуп.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a1f2f3df53414f7f042a444d0482f50c51246e3f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42456494"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="ae0ca-103">Назначение Онпремисесажент для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="ae0ca-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

<span data-ttu-id="ae0ca-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ae0ca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ae0ca-105">Назначение объекта [онпремисесажент](../resources/onpremisesagent.md) объекту [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="ae0ca-105">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ae0ca-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="ae0ca-106">Permissions</span></span>

<span data-ttu-id="ae0ca-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ae0ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ae0ca-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="ae0ca-109">Permission type</span></span>                        | <span data-ttu-id="ae0ca-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="ae0ca-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="ae0ca-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="ae0ca-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ae0ca-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae0ca-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="ae0ca-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="ae0ca-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ae0ca-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae0ca-114">Not supported.</span></span> |
| <span data-ttu-id="ae0ca-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="ae0ca-115">Application</span></span>                            | <span data-ttu-id="ae0ca-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae0ca-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ae0ca-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="ae0ca-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="ae0ca-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ae0ca-118">Request headers</span></span>

| <span data-ttu-id="ae0ca-119">Имя</span><span class="sxs-lookup"><span data-stu-id="ae0ca-119">Name</span></span>          | <span data-ttu-id="ae0ca-120">Описание</span><span class="sxs-lookup"><span data-stu-id="ae0ca-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ae0ca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae0ca-121">Authorization</span></span> | <span data-ttu-id="ae0ca-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="ae0ca-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="ae0ca-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="ae0ca-123">Request body</span></span>

<span data-ttu-id="ae0ca-124">В теле запроса добавьте представление ссылки OData в формате JSON для объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="ae0ca-124">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ae0ca-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae0ca-125">Response</span></span>

<span data-ttu-id="ae0ca-126">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="ae0ca-126">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ae0ca-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="ae0ca-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ae0ca-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="ae0ca-128">Request</span></span>

<span data-ttu-id="ae0ca-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="ae0ca-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ae0ca-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="ae0ca-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascript"></a>[<span data-ttu-id="ae0ca-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ae0ca-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ae0ca-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ae0ca-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="ae0ca-133">В тексте запроса добавьте представление ссылки OData в формате JSON для объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="ae0ca-133">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="ae0ca-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="ae0ca-134">Response</span></span>

<span data-ttu-id="ae0ca-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="ae0ca-135">The following is an example of the response.</span></span>

> <span data-ttu-id="ae0ca-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="ae0ca-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgentGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
