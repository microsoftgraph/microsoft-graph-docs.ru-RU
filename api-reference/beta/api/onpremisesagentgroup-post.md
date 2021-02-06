---
title: Создание onPremisesAgentGroup
description: Создание объекта **onPremisesAgentGroup.**
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2486c83d9e22304f57dbd64d322029fcec201c83
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50136383"
---
# <a name="create-onpremisesagentgroup"></a><span data-ttu-id="48a3e-103">Создание onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="48a3e-103">Create onPremisesAgentGroup</span></span>

<span data-ttu-id="48a3e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="48a3e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48a3e-105">Создание объекта [onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="48a3e-105">Create a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="48a3e-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="48a3e-106">Permissions</span></span>

<span data-ttu-id="48a3e-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="48a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="48a3e-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="48a3e-109">Permission type</span></span>                        | <span data-ttu-id="48a3e-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="48a3e-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="48a3e-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="48a3e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="48a3e-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48a3e-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="48a3e-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="48a3e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48a3e-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48a3e-114">Not supported.</span></span> |
| <span data-ttu-id="48a3e-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="48a3e-115">Application</span></span>                            | <span data-ttu-id="48a3e-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="48a3e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48a3e-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="48a3e-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}/agents
```

## <a name="request-headers"></a><span data-ttu-id="48a3e-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="48a3e-118">Request headers</span></span>

| <span data-ttu-id="48a3e-119">Имя</span><span class="sxs-lookup"><span data-stu-id="48a3e-119">Name</span></span>          | <span data-ttu-id="48a3e-120">Описание</span><span class="sxs-lookup"><span data-stu-id="48a3e-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="48a3e-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="48a3e-121">Authorization</span></span> | <span data-ttu-id="48a3e-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="48a3e-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="48a3e-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="48a3e-123">Request body</span></span>

<span data-ttu-id="48a3e-124">В теле запроса предоставляем представление объекта [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="48a3e-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

## <a name="response"></a><span data-ttu-id="48a3e-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="48a3e-125">Response</span></span>

<span data-ttu-id="48a3e-126">В случае успеха этот метод возвращает код отклика и объект `201 Created` [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="48a3e-126">If successful, this method returns a `201 Created` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="48a3e-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="48a3e-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="48a3e-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="48a3e-128">Request</span></span>

<span data-ttu-id="48a3e-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="48a3e-129">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="48a3e-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="48a3e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_onpremisesagentgroup"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups
```
# <a name="javascript"></a>[<span data-ttu-id="48a3e-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="48a3e-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagent-from-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="48a3e-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="48a3e-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagent-from-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="48a3e-133">В теле запроса предоставляем представление объекта [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) в JSON.</span><span class="sxs-lookup"><span data-stu-id="48a3e-133">In the request body, supply a JSON representation of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

### <a name="response"></a><span data-ttu-id="48a3e-134">Отклик</span><span class="sxs-lookup"><span data-stu-id="48a3e-134">Response</span></span>

<span data-ttu-id="48a3e-135">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="48a3e-135">The following is an example of the response.</span></span>

> <span data-ttu-id="48a3e-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="48a3e-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "4655ed41-1619-4848-92bb-0576d3038682",
    "displayName": "New Group",
    "publishingType": "provisioning",
    "isDefault": false
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create onPremisesAgent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->



