---
title: Назначение Публишедресаурце для Онпремисесажентграуп
description: Назначьте объект **публишедресаурце** объекту **онпремисесажентграуп** .
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 12a30d04b27b0ed098fd12c71fabed90fa321cf8
ms.sourcegitcommit: ee41ba9ec6001716f1a9d575741bbeef577e2473
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/09/2020
ms.locfileid: "43200000"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="77c23-103">Назначение Публишедресаурце для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="77c23-103">Assign publishedResource to onPremisesAgentGroup</span></span>

<span data-ttu-id="77c23-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77c23-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="77c23-105">Назначьте объект [публишедресаурце](../resources/publishedresource.md) объекту [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="77c23-105">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="77c23-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="77c23-106">Permissions</span></span>

<span data-ttu-id="77c23-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="77c23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="77c23-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="77c23-109">Permission type</span></span>                        | <span data-ttu-id="77c23-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="77c23-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="77c23-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="77c23-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="77c23-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="77c23-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="77c23-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="77c23-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77c23-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77c23-114">Not supported.</span></span> |
| <span data-ttu-id="77c23-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="77c23-115">Application</span></span>                            | <span data-ttu-id="77c23-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="77c23-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="77c23-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="77c23-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="77c23-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="77c23-118">Request headers</span></span>

| <span data-ttu-id="77c23-119">Имя</span><span class="sxs-lookup"><span data-stu-id="77c23-119">Name</span></span>          | <span data-ttu-id="77c23-120">Описание</span><span class="sxs-lookup"><span data-stu-id="77c23-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="77c23-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="77c23-121">Authorization</span></span> | <span data-ttu-id="77c23-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="77c23-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="77c23-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="77c23-123">Request body</span></span>

<span data-ttu-id="77c23-124">В тексте запроса добавьте представление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77c23-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="77c23-125">Ответ</span><span class="sxs-lookup"><span data-stu-id="77c23-125">Response</span></span>

<span data-ttu-id="77c23-126">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [публишедресаурце](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="77c23-126">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="77c23-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="77c23-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="77c23-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="77c23-128">Request</span></span>

<span data-ttu-id="77c23-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="77c23-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_onpremisesagentgroup_from_onpremisespublishingprofile"
}-->

```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/publishedResources/1234b780-965f-4149-85c5-a8c73e58b67d/agentGroups/$ref
Content-type: application/json

```http
{
 "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/provisioning/agentGroups/2B032383-897C-42BA-917E-700B6890BDC3/"
}
```

### <a name="response"></a><span data-ttu-id="77c23-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="77c23-130">Response</span></span>

<span data-ttu-id="77c23-131">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="77c23-131">The following is an example of the response.</span></span>

> <span data-ttu-id="77c23-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="77c23-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onPremisesAgentGroup"
} -->

```http
HTTP/1.1 204
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
