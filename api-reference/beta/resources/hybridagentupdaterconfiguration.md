---
title: тип ресурса hybridAgentUpdaterConfiguration
description: тип ресурса hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: c81d48053e7fb26eaee678da4e4b33708717e3c1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722402"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="fba26-103">тип ресурса hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="fba26-103">hybridAgentUpdaterConfiguration resource type</span></span>

<span data-ttu-id="fba26-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fba26-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fba26-105">Администратор клиента может настроить для каждого onPremisesPublishingProfile время, в течение которого агенты могут получать обновления или откладывать обновления агентам.</span><span class="sxs-lookup"><span data-stu-id="fba26-105">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="fba26-106">ГибридAgentUpdaterConfiguration, заданный для onPremisesPublishingProfile, применим ко всем агентам в этом onPremisesPublishingProfile.</span><span class="sxs-lookup"><span data-stu-id="fba26-106">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="fba26-107">Например, для агентов в onPremisesPublishingProfile типа "подготовка" шаги могут быть как ниже.</span><span class="sxs-lookup"><span data-stu-id="fba26-107">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="fba26-108">Администратор клиента может настроить, чтобы не получать какие-либо обновления для агентов предварительного обеспечения в течение следующих n дней.</span><span class="sxs-lookup"><span data-stu-id="fba26-108">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="fba26-109">Администратор клиента может настроить окно обновления (время начала и окончания), в течение которого агенты могут отыскировать обновления.</span><span class="sxs-lookup"><span data-stu-id="fba26-109">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="fba26-110">Администратор клиента может включить allowUpdateConfigurationOverride, переопределяющий configutration updater для агентов provisioning и alows, чтобы получить следующее доступное обновление.</span><span class="sxs-lookup"><span data-stu-id="fba26-110">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="fba26-111">Сведения DateTime/Time, указанные в конфигурации обновления, будут преобразованы в локальный часовой пояс, о чем агент сообщает во время evaluvation.</span><span class="sxs-lookup"><span data-stu-id="fba26-111">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="fba26-112">Обновление агента будет выполняться в приведенном ниже списке приоритетов</span><span class="sxs-lookup"><span data-stu-id="fba26-112">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="fba26-113">Если установлено значение allowUpdateConfigurationOverride, конфигурация обновления, заданная клиентом, будет пропущена, а агент получит обновление при наличии следующей версии агента (приоритет 1).</span><span class="sxs-lookup"><span data-stu-id="fba26-113">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="fba26-114">Если задается обновление отсрочки, агент не будет обновляться до времени отсрочки обновления (приоритет 2).</span><span class="sxs-lookup"><span data-stu-id="fba26-114">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="fba26-115">Если установлено окно обновления, агент будет обновляться только в течение этого 24-часового дня (приоритет 3).</span><span class="sxs-lookup"><span data-stu-id="fba26-115">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="fba26-116">Если клиент не задает допустимую конфигурацию обновления, агент получит обновление при наличии следующей версии агента.</span><span class="sxs-lookup"><span data-stu-id="fba26-116">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="fba26-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="fba26-117">Properties</span></span>

| <span data-ttu-id="fba26-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="fba26-118">Property</span></span>     | <span data-ttu-id="fba26-119">Тип</span><span class="sxs-lookup"><span data-stu-id="fba26-119">Type</span></span>        | <span data-ttu-id="fba26-120">Описание</span><span class="sxs-lookup"><span data-stu-id="fba26-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="fba26-121">allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="fba26-121">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="fba26-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="fba26-122">Boolean</span></span>|<span data-ttu-id="fba26-123">Указывает, будет ли пропущена конфигурация обновления, и агент получит обновление, когда будет доступна следующая версия агента.</span><span class="sxs-lookup"><span data-stu-id="fba26-123">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="fba26-124">deferUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="fba26-124">deferUpdateDateTime</span></span>|<span data-ttu-id="fba26-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fba26-125">DateTimeOffset</span></span>|<span data-ttu-id="fba26-126">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC).</span><span class="sxs-lookup"><span data-stu-id="fba26-126">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fba26-127">Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="fba26-127">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="fba26-128">updateWindow</span><span class="sxs-lookup"><span data-stu-id="fba26-128">updateWindow</span></span>|[<span data-ttu-id="fba26-129">updateWindow</span><span class="sxs-lookup"><span data-stu-id="fba26-129">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="fba26-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fba26-130">JSON representation</span></span>

<span data-ttu-id="fba26-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fba26-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hybridAgentUpdaterConfiguration",
  "baseType": null
}-->

```json
{
  "allowUpdateConfigurationOverride": true,
  "deferUpdateDateTime": "String (timestamp)",
  "updateWindow": {"@odata.type": "microsoft.graph.updateWindow"}
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hybridAgentUpdaterConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


