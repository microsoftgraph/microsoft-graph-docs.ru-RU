---
title: Удаление Публишедресаурце из Онпремисесажентграуп
description: Удаление объекта [публишедресаурце](../resources/publishedresource.md) из объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 898b345fcdc41b3676c27d49f496ea450a966eb0
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841061"
---
# <a name="remove-publishedresource-from-an-onpremisesagentgroup"></a><span data-ttu-id="2be24-103">Удаление Публишедресаурце из Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="2be24-103">Remove publishedResource from an onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2be24-104">Удаление объекта [публишедресаурце](../resources/publishedresource.md) из объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="2be24-104">Remove a [publishedResource](../resources/publishedresource.md) object from an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2be24-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="2be24-105">Permissions</span></span>

<span data-ttu-id="2be24-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2be24-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2be24-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="2be24-108">Permission type</span></span>                        | <span data-ttu-id="2be24-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="2be24-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="2be24-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="2be24-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2be24-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="2be24-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="2be24-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="2be24-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2be24-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2be24-113">Not supported.</span></span> |
| <span data-ttu-id="2be24-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="2be24-114">Application</span></span>                            | <span data-ttu-id="2be24-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2be24-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2be24-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="2be24-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups{id2}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="2be24-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="2be24-117">Request headers</span></span>

| <span data-ttu-id="2be24-118">Имя</span><span class="sxs-lookup"><span data-stu-id="2be24-118">Name</span></span>          | <span data-ttu-id="2be24-119">Описание</span><span class="sxs-lookup"><span data-stu-id="2be24-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2be24-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="2be24-120">Authorization</span></span> | <span data-ttu-id="2be24-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="2be24-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2be24-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="2be24-122">Request body</span></span>

<span data-ttu-id="2be24-123">Не указывайте текст запроса для этого метода.</span><span class="sxs-lookup"><span data-stu-id="2be24-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2be24-124">Ответ</span><span class="sxs-lookup"><span data-stu-id="2be24-124">Response</span></span>

<span data-ttu-id="2be24-125">В случае успешного выполнения этот метод возвращает код отклика `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2be24-125">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="2be24-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="2be24-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2be24-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="2be24-127">Request</span></span>

<span data-ttu-id="2be24-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="2be24-128">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_publishedresource"
}-->

```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/8832388F-3814-4952-B288-FFB62081FE25/$ref
```

### <a name="response"></a><span data-ttu-id="2be24-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="2be24-129">Response</span></span>

<span data-ttu-id="2be24-130">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="2be24-130">The following is an example of the response.</span></span>

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
  "description": "Delete publishedResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
