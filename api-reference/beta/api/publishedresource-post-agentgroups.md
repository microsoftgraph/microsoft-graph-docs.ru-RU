---
title: Назначение Публишедресаурце для Онпремисесажентграуп
description: Назначьте объект **публишедресаурце** объекту **онпремисесажентграуп** .
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9ec20b1208906129e5559307fc347e9d39c6dd7e
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840970"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="04b79-103">Назначение Публишедресаурце для Онпремисесажентграуп</span><span class="sxs-lookup"><span data-stu-id="04b79-103">Assign publishedResource to onPremisesAgentGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04b79-104">Назначьте объект [публишедресаурце](../resources/publishedresource.md) объекту [онпремисесажентграуп](../resources/onpremisesagentgroup.md) .</span><span class="sxs-lookup"><span data-stu-id="04b79-104">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="04b79-105">Разрешения</span><span class="sxs-lookup"><span data-stu-id="04b79-105">Permissions</span></span>

<span data-ttu-id="04b79-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="04b79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="04b79-108">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="04b79-108">Permission type</span></span>                        | <span data-ttu-id="04b79-109">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="04b79-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="04b79-110">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="04b79-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="04b79-111">Онпремисеспублишингпрофилес. ReadWrite. ALL</span><span class="sxs-lookup"><span data-stu-id="04b79-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="04b79-112">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="04b79-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04b79-113">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b79-113">Not supported.</span></span> |
| <span data-ttu-id="04b79-114">Для приложений</span><span class="sxs-lookup"><span data-stu-id="04b79-114">Application</span></span>                            | <span data-ttu-id="04b79-115">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04b79-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="04b79-116">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="04b79-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="04b79-117">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="04b79-117">Request headers</span></span>

| <span data-ttu-id="04b79-118">Имя</span><span class="sxs-lookup"><span data-stu-id="04b79-118">Name</span></span>          | <span data-ttu-id="04b79-119">Описание</span><span class="sxs-lookup"><span data-stu-id="04b79-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="04b79-120">Авторизация</span><span class="sxs-lookup"><span data-stu-id="04b79-120">Authorization</span></span> | <span data-ttu-id="04b79-121">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="04b79-121">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="04b79-122">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="04b79-122">Request body</span></span>

<span data-ttu-id="04b79-123">В тексте запроса добавьте представление объекта [онпремисесажентграуп](../resources/onpremisesagentgroup.md) в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04b79-123">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04b79-124">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b79-124">Response</span></span>

<span data-ttu-id="04b79-125">В случае успешного выполнения этот метод возвращает `201 Created` код отклика и объект [публишедресаурце](../resources/publishedresource.md) в тексте отклика.</span><span class="sxs-lookup"><span data-stu-id="04b79-125">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="04b79-126">Примеры</span><span class="sxs-lookup"><span data-stu-id="04b79-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="04b79-127">Запрос</span><span class="sxs-lookup"><span data-stu-id="04b79-127">Request</span></span>

<span data-ttu-id="04b79-128">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="04b79-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04b79-129">Отклик</span><span class="sxs-lookup"><span data-stu-id="04b79-129">Response</span></span>

<span data-ttu-id="04b79-130">Ниже приведен пример отклика.</span><span class="sxs-lookup"><span data-stu-id="04b79-130">The following is an example of the response.</span></span>

> <span data-ttu-id="04b79-p102">**Примечание.** Представленный здесь объект отклика может быть сокращен для удобочитаемости. При фактическом вызове будут возвращены все свойства.</span><span class="sxs-lookup"><span data-stu-id="04b79-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
