---
title: Назначение publishedResource onPremisesAgentGroup
description: '**Назначьте объект publishedResource** **объекту onPremisesAgentGroup.**'
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 3cbd9e434701cad6ac7eff47daed6080c5979863
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055171"
---
# <a name="assign-publishedresource-to-onpremisesagentgroup"></a><span data-ttu-id="b068b-103">Назначение publishedResource onPremisesAgentGroup</span><span class="sxs-lookup"><span data-stu-id="b068b-103">Assign publishedResource to onPremisesAgentGroup</span></span>

<span data-ttu-id="b068b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b068b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b068b-105">[Назначьте объект publishedResource](../resources/publishedresource.md) [объекту OnPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b068b-105">Assign a [publishedResource](../resources/publishedresource.md) object to [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b068b-106">Разрешения</span><span class="sxs-lookup"><span data-stu-id="b068b-106">Permissions</span></span>

<span data-ttu-id="b068b-p101">Для вызова этого API требуется одно из указанных ниже разрешений. Дополнительные сведения, включая сведения о том, как выбрать разрешения, см. в статье [Разрешения](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b068b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b068b-109">Тип разрешения</span><span class="sxs-lookup"><span data-stu-id="b068b-109">Permission type</span></span>                        | <span data-ttu-id="b068b-110">Разрешения (в порядке повышения привилегий)</span><span class="sxs-lookup"><span data-stu-id="b068b-110">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="b068b-111">Делегированные (рабочая или учебная учетная запись)</span><span class="sxs-lookup"><span data-stu-id="b068b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b068b-112">OnPremisesPublishingProfiles.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b068b-112">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="b068b-113">Делегированные (личная учетная запись Майкрософт)</span><span class="sxs-lookup"><span data-stu-id="b068b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b068b-114">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b068b-114">Not supported.</span></span> |
| <span data-ttu-id="b068b-115">Для приложений</span><span class="sxs-lookup"><span data-stu-id="b068b-115">Application</span></span>                            | <span data-ttu-id="b068b-116">Не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b068b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b068b-117">HTTP-запрос</span><span class="sxs-lookup"><span data-stu-id="b068b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST ~/onPremisesPublishingProfiles/{publishingType}/publishedResources/{id1}/agentGroups/$ref
```

## <a name="request-headers"></a><span data-ttu-id="b068b-118">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="b068b-118">Request headers</span></span>

| <span data-ttu-id="b068b-119">Имя</span><span class="sxs-lookup"><span data-stu-id="b068b-119">Name</span></span>          | <span data-ttu-id="b068b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="b068b-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b068b-121">Авторизация</span><span class="sxs-lookup"><span data-stu-id="b068b-121">Authorization</span></span> | <span data-ttu-id="b068b-122">Bearer {token}</span><span class="sxs-lookup"><span data-stu-id="b068b-122">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="b068b-123">Тело запроса</span><span class="sxs-lookup"><span data-stu-id="b068b-123">Request body</span></span>

<span data-ttu-id="b068b-124">В теле запроса поставляем представление JSON объекта [onPremisesAgentGroup.](../resources/onpremisesagentgroup.md)</span><span class="sxs-lookup"><span data-stu-id="b068b-124">In the request body, supply a JSON representation of an [onPremisesAgentGroup](../resources/onpremisesagentgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="b068b-125">Отклик</span><span class="sxs-lookup"><span data-stu-id="b068b-125">Response</span></span>

<span data-ttu-id="b068b-126">В случае успешной работы этот метод возвращает код отклика и `201 Created` [объект publishedResource](../resources/publishedresource.md) в тексте ответа.</span><span class="sxs-lookup"><span data-stu-id="b068b-126">If successful, this method returns a `201 Created` response code and a [publishedResource](../resources/publishedresource.md) object  in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b068b-127">Примеры</span><span class="sxs-lookup"><span data-stu-id="b068b-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b068b-128">Запрос</span><span class="sxs-lookup"><span data-stu-id="b068b-128">Request</span></span>

<span data-ttu-id="b068b-129">Ниже приведен пример запроса.</span><span class="sxs-lookup"><span data-stu-id="b068b-129">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b068b-130">Отклик</span><span class="sxs-lookup"><span data-stu-id="b068b-130">Response</span></span>

<span data-ttu-id="b068b-131">Ниже приведен пример ответа.</span><span class="sxs-lookup"><span data-stu-id="b068b-131">The following is an example of the response.</span></span>

> <span data-ttu-id="b068b-132">**Примечание.** Объект отклика, показанный здесь, может быть сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="b068b-132">**Note:** The response object shown here might be shortened for readability.</span></span>

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



