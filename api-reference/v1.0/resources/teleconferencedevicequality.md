---
title: Тип ресурса Телеконференцедевицекуалити
description: Представляет данные качества на уровне сеанса видеоконференций для видеоконференций.
localization_priority: Normal
author: dongkyun
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: c96382644793b57dd0eaa7b0f95213897e6068ce
ms.sourcegitcommit: 3834b7b0287ee71668c52c42d3465ca19366e678
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/01/2020
ms.locfileid: "43082772"
---
# <a name="teleconferencedevicequality-resource-type"></a><span data-ttu-id="565ab-103">Тип ресурса Телеконференцедевицекуалити</span><span class="sxs-lookup"><span data-stu-id="565ab-103">teleconferenceDeviceQuality resource type</span></span>

<span data-ttu-id="565ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="565ab-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="565ab-105">Представляет данные качества на уровне сеанса видеоконференций для видеоконференций.</span><span class="sxs-lookup"><span data-stu-id="565ab-105">Represents video teleconferencing device session-level quality data.</span></span>

## <a name="properties"></a><span data-ttu-id="565ab-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="565ab-106">Properties</span></span>

| <span data-ttu-id="565ab-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="565ab-107">Property</span></span>     | <span data-ttu-id="565ab-108">Тип</span><span class="sxs-lookup"><span data-stu-id="565ab-108">Type</span></span>        | <span data-ttu-id="565ab-109">Описание</span><span class="sxs-lookup"><span data-stu-id="565ab-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="565ab-110">callChainId</span><span class="sxs-lookup"><span data-stu-id="565ab-110">callChainId</span></span>|<span data-ttu-id="565ab-111">GUID</span><span class="sxs-lookup"><span data-stu-id="565ab-111">Guid</span></span>|<span data-ttu-id="565ab-112">Уникальный идентификатор для всех вызовов участников в конференции или уникальный идентификатор для двух вызовов участников в вызове P2P.</span><span class="sxs-lookup"><span data-stu-id="565ab-112">A unique identifier for all  the participant calls in a conference or a unique identifier for two participant calls in P2P call.</span></span> <span data-ttu-id="565ab-113">Необходимо скопировать из `Microsoft.Graph.Call.CallChainId`.</span><span class="sxs-lookup"><span data-stu-id="565ab-113">This needs to be copied over from `Microsoft.Graph.Call.CallChainId`.</span></span>|
|<span data-ttu-id="565ab-114">клаудсервицедеплойментенвиронмент</span><span class="sxs-lookup"><span data-stu-id="565ab-114">cloudServiceDeploymentEnvironment</span></span>|<span data-ttu-id="565ab-115">String</span><span class="sxs-lookup"><span data-stu-id="565ab-115">String</span></span>|<span data-ttu-id="565ab-116">Географическая область, в которой развернута служба, `ProdNoam`например.</span><span class="sxs-lookup"><span data-stu-id="565ab-116">A geo-region where the service is deployed, such as `ProdNoam`.</span></span>|
|<span data-ttu-id="565ab-117">клаудсервицедеплойментид</span><span class="sxs-lookup"><span data-stu-id="565ab-117">cloudServiceDeploymentId</span></span>|<span data-ttu-id="565ab-118">String</span><span class="sxs-lookup"><span data-stu-id="565ab-118">String</span></span>|<span data-ttu-id="565ab-119">Уникальный идентификатор развертывания, назначенный Azure.</span><span class="sxs-lookup"><span data-stu-id="565ab-119">A unique deployment identifier assigned by Azure.</span></span>|
|<span data-ttu-id="565ab-120">клаудсервицеинстанценаме</span><span class="sxs-lookup"><span data-stu-id="565ab-120">cloudServiceInstanceName</span></span>|<span data-ttu-id="565ab-121">String</span><span class="sxs-lookup"><span data-stu-id="565ab-121">String</span></span>|<span data-ttu-id="565ab-122">Имя развернутого экземпляра облачной службы Azure, `FrontEnd_IN_3`например.</span><span class="sxs-lookup"><span data-stu-id="565ab-122">The Azure deployed cloud service instance name, such as `FrontEnd_IN_3`.</span></span>|
|<span data-ttu-id="565ab-123">клаудсервиценаме</span><span class="sxs-lookup"><span data-stu-id="565ab-123">cloudServiceName</span></span>|<span data-ttu-id="565ab-124">String</span><span class="sxs-lookup"><span data-stu-id="565ab-124">String</span></span>|<span data-ttu-id="565ab-125">Имя развернутой облачной службы Azure, `contoso.cloudapp.net`например.</span><span class="sxs-lookup"><span data-stu-id="565ab-125">The Azure deployed cloud service name, such as `contoso.cloudapp.net`.</span></span>|
|<span data-ttu-id="565ab-126">девицедескриптион</span><span class="sxs-lookup"><span data-stu-id="565ab-126">deviceDescription</span></span>|<span data-ttu-id="565ab-127">String</span><span class="sxs-lookup"><span data-stu-id="565ab-127">String</span></span>|<span data-ttu-id="565ab-128">Любое дополнительное описание, например `VTC Bldg 30/21`.</span><span class="sxs-lookup"><span data-stu-id="565ab-128">Any additional description, such as `VTC Bldg 30/21`.</span></span>|
|<span data-ttu-id="565ab-129">deviceName</span><span class="sxs-lookup"><span data-stu-id="565ab-129">deviceName</span></span>|<span data-ttu-id="565ab-130">String</span><span class="sxs-lookup"><span data-stu-id="565ab-130">String</span></span>|<span data-ttu-id="565ab-131">Имя агента мультимедиа пользователя, например `Cisco SX80`.</span><span class="sxs-lookup"><span data-stu-id="565ab-131">The user media agent name, such as `Cisco SX80`.</span></span>|
|<span data-ttu-id="565ab-132">медиалегид</span><span class="sxs-lookup"><span data-stu-id="565ab-132">mediaLegId</span></span>|<span data-ttu-id="565ab-133">GUID</span><span class="sxs-lookup"><span data-stu-id="565ab-133">Guid</span></span>|<span data-ttu-id="565ab-134">Уникальный идентификатор для конкретной точки носителя участника в Конференции.</span><span class="sxs-lookup"><span data-stu-id="565ab-134">A unique identifier for a specific media leg of a participant in a conference.</span></span>  <span data-ttu-id="565ab-135">Если происходит переопределение, у одного участника может быть несколько идентификаторов носителей.</span><span class="sxs-lookup"><span data-stu-id="565ab-135">One participant can have multiple media leg identifiers if retargeting happens.</span></span> <span data-ttu-id="565ab-136">Партнер Кви назначает это значение.</span><span class="sxs-lookup"><span data-stu-id="565ab-136">CVI partner assigns this value.</span></span>|
|<span data-ttu-id="565ab-137">медиакуалитилист</span><span class="sxs-lookup"><span data-stu-id="565ab-137">mediaQualityList</span></span>|<span data-ttu-id="565ab-138">Коллекция [телеконференцедевицемедиакуалити](teleconferencedevicemediaquality.md)</span><span class="sxs-lookup"><span data-stu-id="565ab-138">[teleconferenceDeviceMediaQuality](teleconferencedevicemediaquality.md) collection</span></span>|<span data-ttu-id="565ab-139">Список качеств мультимедиа в сеансе мультимедиа (вызов), например качество звука, качество видео и/или общий доступ к экрану.</span><span class="sxs-lookup"><span data-stu-id="565ab-139">The list of media qualities in a media session (call), such as audio quality, video quality, and/or screen sharing quality.</span></span>|
|<span data-ttu-id="565ab-140">партиЦипантид</span><span class="sxs-lookup"><span data-stu-id="565ab-140">participantId</span></span>|<span data-ttu-id="565ab-141">GUID</span><span class="sxs-lookup"><span data-stu-id="565ab-141">Guid</span></span>|<span data-ttu-id="565ab-142">Уникальный идентификатор определенного участника в Конференции.</span><span class="sxs-lookup"><span data-stu-id="565ab-142">A unique identifier for a specific participant in a conference.</span></span> <span data-ttu-id="565ab-143">Партнеру Кви необходимо скопировать `Call.MyParticipantId` значение этого свойства.</span><span class="sxs-lookup"><span data-stu-id="565ab-143">The CVI partner needs to copy over `Call.MyParticipantId` to this property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="565ab-144">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="565ab-144">JSON representation</span></span>

<span data-ttu-id="565ab-145">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="565ab-145">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.teleconferenceDeviceQuality",
  "baseType": null
}-->

```json
{
  "callChainId": "Guid",
  "cloudServiceDeploymentEnvironment": "String",
  "cloudServiceDeploymentId": "String",
  "cloudServiceInstanceName": "String",
  "cloudServiceName": "String",
  "deviceDescription": "String",
  "deviceName": "String",
  "mediaLegId": "Guid",
  "mediaQualityList": [{"@odata.type": "microsoft.graph.teleconferenceDeviceMediaQuality"}],
  "participantId": "Guid"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "teleconferenceDeviceQuality resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
