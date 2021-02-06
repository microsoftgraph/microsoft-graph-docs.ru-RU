---
title: Назначение onPremisesAgent для onPremisesAgentGroup
description: Назначьте onPremisesAgent onPremisesAgentGroup.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 6e4899885573abebda0f5dfb23bdadf852673c02
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136428"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="fc20a-103">Назначение onPremisesAgent для onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="fc20a-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

<span data-ttu-id="fc20a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc20a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc20a-105">[Назначьте onPremisesAgent](../resources/onpremisesagent.md) [объекту onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="fc20a-105">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc20a-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="fc20a-106">Permissions</span></span>

<span data-ttu-id="fc20a-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fc20a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc20a-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="fc20a-109">Permission type</span></span>                        | <span data-ttu-id="fc20a-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="fc20a-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc20a-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="fc20a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="fc20a-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc20a-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="fc20a-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="fc20a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc20a-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc20a-114">Not supported.</span></span> |
| <span data-ttu-id="fc20a-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="fc20a-115">Application</span></span>                            | <span data-ttu-id="fc20a-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc20a-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc20a-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="fc20a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="fc20a-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="fc20a-118">Request headers</span></span>

| <span data-ttu-id="fc20a-119">Имя</span><span class="sxs-lookup"><span data-stu-id="fc20a-119">Name</span></span>          | <span data-ttu-id="fc20a-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fc20a-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="fc20a-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="fc20a-121">Authorization</span></span> | <span data-ttu-id="fc20a-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="fc20a-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc20a-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="fc20a-123">Request body</span></span>

<span data-ttu-id="fc20a-124">В теле запроса предопустим представление ссылки OData в JSON для объекта [onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="fc20a-124">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fc20a-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc20a-125">Response</span></span>

<span data-ttu-id="fc20a-126">В случае успеха этот метод возвращает код отклика и новый объект `201 Created` [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="fc20a-126">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc20a-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="fc20a-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc20a-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="fc20a-128">Request</span></span>

<span data-ttu-id="fc20a-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="fc20a-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc20a-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc20a-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascript"></a>[<span data-ttu-id="fc20a-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc20a-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc20a-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc20a-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="fc20a-133">В теле запроса предоставляем ссылку OData в JSON на объект [onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="fc20a-133">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="fc20a-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="fc20a-134">Response</span></span>

<span data-ttu-id="fc20a-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="fc20a-135">The following is an example of the response.</span></span>

> <span data-ttu-id="fc20a-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="fc20a-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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



