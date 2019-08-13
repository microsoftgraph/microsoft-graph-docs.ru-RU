---
title: Назначение Онпремисесажент для Онпремисесажентграуп
description: Назначьте Онпремисесажент для Онпремисесажентграуп.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 000385e1b2faad98bee217d2709f5516ea40b6b6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342644"
---
# <a name="assign-onpremisesagent-to-onpremisesagentgroup"></a><span data-ttu-id="6a7de-103">Назначение Онпремисесажент для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="6a7de-103">Assign onPremisesAgent to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a7de-104">Назначение объекта [онпремисесажент](../resources/onpremisesagent.md) объекту [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6a7de-104">Assign an [onPremisesAgent](../resources/onpremisesagent.md) to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6a7de-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6a7de-105">Permissions</span></span>

<span data-ttu-id="6a7de-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a7de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a7de-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6a7de-108">Permission type</span></span>                        | <span data-ttu-id="6a7de-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6a7de-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a7de-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6a7de-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a7de-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6a7de-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6a7de-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6a7de-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a7de-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a7de-113">Not supported.</span></span> |
| <span data-ttu-id="6a7de-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6a7de-114">Application</span></span>                            | <span data-ttu-id="6a7de-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a7de-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a7de-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6a7de-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agents/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="6a7de-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6a7de-117">Request headers</span></span>

| <span data-ttu-id="6a7de-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6a7de-118">Name</span></span>          | <span data-ttu-id="6a7de-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6a7de-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6a7de-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6a7de-120">Authorization</span></span> | <span data-ttu-id="6a7de-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6a7de-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a7de-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6a7de-122">Request body</span></span>

<span data-ttu-id="6a7de-123">В теле запроса добавьте представление ссылки OData в формате JSON для объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6a7de-123">In the request body, supply a JSON representation of an OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6a7de-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a7de-124">Response</span></span>

<span data-ttu-id="6a7de-125">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и новый объект [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6a7de-125">If successful, this method returns a `201 Created` response code and a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a7de-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="6a7de-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a7de-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="6a7de-127">Request</span></span>

<span data-ttu-id="6a7de-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6a7de-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6a7de-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a7de-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisesagent"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agents/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6a7de-130">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6a7de-130">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagentgroup-from-onpremisesagent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6a7de-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="6a7de-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagentgroup-from-onpremisesagent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="6a7de-132">В тексте запроса добавьте представление ссылки OData в формате JSON для объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6a7de-132">In the request body, supply a JSON representation of OData reference to an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```http
{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/"
}
```

### <a name="response"></a><span data-ttu-id="6a7de-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="6a7de-133">Response</span></span>

<span data-ttu-id="6a7de-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6a7de-134">The following is an example of the response.</span></span>

> <span data-ttu-id="6a7de-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6a7de-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
