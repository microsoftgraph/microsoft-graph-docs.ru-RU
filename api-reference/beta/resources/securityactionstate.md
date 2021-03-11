---
title: тип ресурса securityActionState
description: Представляет историю изменений состояния securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 6a2fecbc05c9987ee8daec8fa017d728a2d03ed3
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722092"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="d344b-103">тип ресурса securityActionState</span><span class="sxs-lookup"><span data-stu-id="d344b-103">securityActionState resource type</span></span>

<span data-ttu-id="d344b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d344b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d344b-105">Представляет историю изменений состояния securityAction.</span><span class="sxs-lookup"><span data-stu-id="d344b-105">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="d344b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d344b-106">Properties</span></span>

| <span data-ttu-id="d344b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d344b-107">Property</span></span>     | <span data-ttu-id="d344b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d344b-108">Type</span></span>        | <span data-ttu-id="d344b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d344b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d344b-110">appId</span><span class="sxs-lookup"><span data-stu-id="d344b-110">appId</span></span>|<span data-ttu-id="d344b-111">String</span><span class="sxs-lookup"><span data-stu-id="d344b-111">String</span></span>|<span data-ttu-id="d344b-112">ID приложения вызываемого приложения, которое представило обновление (PATCH) к действию.</span><span class="sxs-lookup"><span data-stu-id="d344b-112">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="d344b-113">Маркер должен быть извлечен из маркера auth и не вошел `appId` вручную с помощью вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="d344b-113">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="d344b-114">status</span><span class="sxs-lookup"><span data-stu-id="d344b-114">status</span></span>|<span data-ttu-id="d344b-115">String</span><span class="sxs-lookup"><span data-stu-id="d344b-115">String</span></span>| <span data-ttu-id="d344b-116">Состояние securityAction в этом обновлении.</span><span class="sxs-lookup"><span data-stu-id="d344b-116">Status of the securityAction in this update.</span></span> <span data-ttu-id="d344b-117">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="d344b-117">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="d344b-118">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="d344b-118">updatedDateTime</span></span>|<span data-ttu-id="d344b-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d344b-119">DateTimeOffset</span></span>| <span data-ttu-id="d344b-120">Timestamp при обновлении actionState.</span><span class="sxs-lookup"><span data-stu-id="d344b-120">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="d344b-121">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="d344b-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="d344b-122">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="d344b-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="d344b-123">user</span><span class="sxs-lookup"><span data-stu-id="d344b-123">user</span></span>|<span data-ttu-id="d344b-124">String</span><span class="sxs-lookup"><span data-stu-id="d344b-124">String</span></span>|<span data-ttu-id="d344b-125">Основное имя пользователя пользователя, который отправил в действие обновление (PATCH).</span><span class="sxs-lookup"><span data-stu-id="d344b-125">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="d344b-126">Маркер должен быть извлечен из маркера auth и не вошел `user` вручную с помощью вызываемого приложения.</span><span class="sxs-lookup"><span data-stu-id="d344b-126">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d344b-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d344b-127">JSON representation</span></span>

<span data-ttu-id="d344b-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d344b-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityActionState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityActionState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


