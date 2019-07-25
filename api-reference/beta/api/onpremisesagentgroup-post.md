---
title: Создание Онпремисесажентграуп
description: Создание нового объекта **онпремисесажентграуп** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1771976abc56bb2b39850dcc925003df8965192e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878315"
---
# <a name="create-onpremisesagentgroup"></a><span data-ttu-id="c2c5b-103">Создание Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="c2c5b-103">Create onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2c5b-104">Создание нового объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="c2c5b-104">Create a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2c5b-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="c2c5b-105">Permissions</span></span>

<span data-ttu-id="c2c5b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2c5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c2c5b-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="c2c5b-108">Permission type</span></span>                        | <span data-ttu-id="c2c5b-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="c2c5b-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2c5b-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="c2c5b-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="c2c5b-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="c2c5b-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="c2c5b-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="c2c5b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2c5b-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2c5b-113">Not supported.</span></span> |
| <span data-ttu-id="c2c5b-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="c2c5b-114">Application</span></span>                            | <span data-ttu-id="c2c5b-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2c5b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2c5b-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="c2c5b-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}/agents
```

## <a name="request-headers"></a><span data-ttu-id="c2c5b-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="c2c5b-117">Request headers</span></span>

| <span data-ttu-id="c2c5b-118">Имя</span><span class="sxs-lookup"><span data-stu-id="c2c5b-118">Name</span></span>          | <span data-ttu-id="c2c5b-119">Описание</span><span class="sxs-lookup"><span data-stu-id="c2c5b-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="c2c5b-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="c2c5b-120">Authorization</span></span> | <span data-ttu-id="c2c5b-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="c2c5b-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c2c5b-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="c2c5b-122">Request body</span></span>

<span data-ttu-id="c2c5b-123">В тексте запроса добавьте представление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2c5b-123">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

## <a name="response"></a><span data-ttu-id="c2c5b-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2c5b-124">Response</span></span>

<span data-ttu-id="c2c5b-125">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="c2c5b-125">If successful, this method returns a `201 Created` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c2c5b-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="c2c5b-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c2c5b-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="c2c5b-127">Request</span></span>

<span data-ttu-id="c2c5b-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="c2c5b-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c2c5b-129">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2c5b-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_onpremisesagentgroup"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups
```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2c5b-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2c5b-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-onpremisesagent-from-onpremisesagentgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2c5b-131">Цель — C</span><span class="sxs-lookup"><span data-stu-id="c2c5b-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-onpremisesagent-from-onpremisesagentgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<span data-ttu-id="c2c5b-132">В тексте запроса добавьте представление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2c5b-132">In the request body, supply a JSON representation of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

### <a name="response"></a><span data-ttu-id="c2c5b-133">Отклик</span><span class="sxs-lookup"><span data-stu-id="c2c5b-133">Response</span></span>

<span data-ttu-id="c2c5b-134">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="c2c5b-134">The following is an example of the response.</span></span>

> <span data-ttu-id="c2c5b-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="c2c5b-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
