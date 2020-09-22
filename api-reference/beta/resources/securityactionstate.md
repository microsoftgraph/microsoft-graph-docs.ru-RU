---
title: Тип ресурса Секуритяктионстате
description: Представляет историю изменений состояния securityAction.
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: ba22a03f4d4a6d03b0093ed28b8c54a7c095d037
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47988865"
---
# <a name="securityactionstate-resource-type"></a><span data-ttu-id="a3db5-103">Тип ресурса Секуритяктионстате</span><span class="sxs-lookup"><span data-stu-id="a3db5-103">securityActionState resource type</span></span>

<span data-ttu-id="a3db5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3db5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3db5-105">Представляет историю изменений состояния securityAction.</span><span class="sxs-lookup"><span data-stu-id="a3db5-105">Represents the history of securityAction state changes.</span></span>

## <a name="properties"></a><span data-ttu-id="a3db5-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a3db5-106">Properties</span></span>

| <span data-ttu-id="a3db5-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a3db5-107">Property</span></span>     | <span data-ttu-id="a3db5-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a3db5-108">Type</span></span>        | <span data-ttu-id="a3db5-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a3db5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a3db5-110">appId</span><span class="sxs-lookup"><span data-stu-id="a3db5-110">appId</span></span>|<span data-ttu-id="a3db5-111">String</span><span class="sxs-lookup"><span data-stu-id="a3db5-111">String</span></span>|<span data-ttu-id="a3db5-112">Идентификатор приложения вызывающего приложения, отправившего обновление (исправление) действию.</span><span class="sxs-lookup"><span data-stu-id="a3db5-112">The Application ID of the calling application that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="a3db5-113">Его `appId` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="a3db5-113">The `appId` should be extracted from the auth token and not entered manually by the calling application.</span></span>|
|<span data-ttu-id="a3db5-114">status</span><span class="sxs-lookup"><span data-stu-id="a3db5-114">status</span></span>|<span data-ttu-id="a3db5-115">String</span><span class="sxs-lookup"><span data-stu-id="a3db5-115">String</span></span>| <span data-ttu-id="a3db5-116">Состояние securityAction в этом обновлении.</span><span class="sxs-lookup"><span data-stu-id="a3db5-116">Status of the securityAction in this update.</span></span> <span data-ttu-id="a3db5-117">Возможные значения: `NotStarted`, `Running`, `Completed`, `Failed`.</span><span class="sxs-lookup"><span data-stu-id="a3db5-117">Possible values are: `NotStarted`, `Running`, `Completed`, `Failed`.</span></span>|
|<span data-ttu-id="a3db5-118">упдатеддатетиме</span><span class="sxs-lookup"><span data-stu-id="a3db5-118">updatedDateTime</span></span>|<span data-ttu-id="a3db5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3db5-119">DateTimeOffset</span></span>| <span data-ttu-id="a3db5-120">Временная метка при обновлении actionState.</span><span class="sxs-lookup"><span data-stu-id="a3db5-120">Timestamp when the actionState was updated.</span></span> <span data-ttu-id="a3db5-121">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="a3db5-121">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a3db5-122">Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a3db5-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="a3db5-123">user</span><span class="sxs-lookup"><span data-stu-id="a3db5-123">user</span></span>|<span data-ttu-id="a3db5-124">String</span><span class="sxs-lookup"><span data-stu-id="a3db5-124">String</span></span>|<span data-ttu-id="a3db5-125">Имя участника-пользователя, который выполнил вход в действие при отправке обновления (исправления).</span><span class="sxs-lookup"><span data-stu-id="a3db5-125">The user principal name of the signed-in user that submitted an update (PATCH) to the action.</span></span> <span data-ttu-id="a3db5-126">Его `user` необходимо извлечь из маркера проверки подлинности и не вводить вручную вызывающим приложением.</span><span class="sxs-lookup"><span data-stu-id="a3db5-126">The `user` should be extracted from the auth token and not entered manually by the calling application.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3db5-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a3db5-127">JSON representation</span></span>

<span data-ttu-id="a3db5-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a3db5-128">The following is a JSON representation of the resource.</span></span>

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


