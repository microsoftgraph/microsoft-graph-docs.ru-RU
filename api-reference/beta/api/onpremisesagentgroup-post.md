---
title: Создание Онпремисесажентграуп
description: Создание нового объекта **онпремисесажентграуп** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 752081e6b50460e8185f4bddddce603bf54e5d86
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841096"
---
# <a name="create-onpremisesagentgroup"></a><span data-ttu-id="6d7d5-103">Создание Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="6d7d5-103">Create onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d7d5-104">Создание нового объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="6d7d5-104">Create a new [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d7d5-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="6d7d5-105">Permissions</span></span>

<span data-ttu-id="6d7d5-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6d7d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6d7d5-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="6d7d5-108">Permission type</span></span>                        | <span data-ttu-id="6d7d5-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="6d7d5-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d7d5-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="6d7d5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="6d7d5-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="6d7d5-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="6d7d5-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="6d7d5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d7d5-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d7d5-113">Not supported.</span></span> |
| <span data-ttu-id="6d7d5-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="6d7d5-114">Application</span></span>                            | <span data-ttu-id="6d7d5-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d7d5-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6d7d5-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="6d7d5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/agentGroups/{id}/agents
```

## <a name="request-headers"></a><span data-ttu-id="6d7d5-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="6d7d5-117">Request headers</span></span>

| <span data-ttu-id="6d7d5-118">Имя</span><span class="sxs-lookup"><span data-stu-id="6d7d5-118">Name</span></span>          | <span data-ttu-id="6d7d5-119">Описание</span><span class="sxs-lookup"><span data-stu-id="6d7d5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6d7d5-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="6d7d5-120">Authorization</span></span> | <span data-ttu-id="6d7d5-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="6d7d5-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="6d7d5-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="6d7d5-122">Request body</span></span>

<span data-ttu-id="6d7d5-123">В тексте запроса добавьте представление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d7d5-123">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

## <a name="response"></a><span data-ttu-id="6d7d5-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d7d5-124">Response</span></span>

<span data-ttu-id="6d7d5-125">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="6d7d5-125">If successful, this method returns a `201 Created` response code and an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6d7d5-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="6d7d5-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6d7d5-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="6d7d5-127">Request</span></span>

<span data-ttu-id="6d7d5-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="6d7d5-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagent_from_onpremisesagentgroup"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups
```

<span data-ttu-id="6d7d5-129">В тексте запроса добавьте представление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d7d5-129">In the request body, supply a JSON representation of [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

```json
{
    "displayName": "New Group"
}
```

### <a name="response"></a><span data-ttu-id="6d7d5-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="6d7d5-130">Response</span></span>

<span data-ttu-id="6d7d5-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="6d7d5-131">The following is an example of the response.</span></span>

> <span data-ttu-id="6d7d5-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="6d7d5-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
