---
title: Тип ресурса hybridAgentUpdaterConfiguration
description: Тип ресурса hybridAgentUpdaterConfiguration.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 39b378397b18337c660e76b815a80c9db398f950
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128605"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="60beb-103">Тип ресурса hybridAgentUpdaterConfiguration</span><span class="sxs-lookup"><span data-stu-id="60beb-103">hybridAgentUpdaterConfiguration resource type</span></span>

<span data-ttu-id="60beb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60beb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="60beb-105">Администратор клиента может настроить для каждого onPremisesPublishingProfile период времени, в течение которого агенты могут получать обновления или откладывать обновления для агентов.</span><span class="sxs-lookup"><span data-stu-id="60beb-105">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="60beb-106">Гибридная системаAgentUpdaterConfiguration, указанная для onPremisesPublishingProfile, применима ко всем агентам в этом onPremisesPublishingProfile.</span><span class="sxs-lookup"><span data-stu-id="60beb-106">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="60beb-107">Например, для агентов в onPremisesPublishingProfile типа "подготовка" шаги могут быть, как пошаговом примере ниже.</span><span class="sxs-lookup"><span data-stu-id="60beb-107">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="60beb-108">Администратор клиента может настроить не получать обновления агентов предоставления в течение следующих n дней.</span><span class="sxs-lookup"><span data-stu-id="60beb-108">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="60beb-109">Администратор клиента может настроить окно обновления (время начала и окончания), в течение которого агенты могут пересылать обновления.</span><span class="sxs-lookup"><span data-stu-id="60beb-109">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="60beb-110">Администратор клиента может включить allowUpdateConfigurationOverride, который переопределит конфигурирование средства обновления для агентов предоставления и отобразит для них получение следующего доступного обновления.</span><span class="sxs-lookup"><span data-stu-id="60beb-110">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="60beb-111">Сведения о времени и времени, указанные в конфигурации средства обновления, будут преобразованы в локальный часовой пояс, сообщаемой агентом во время evaluvation.</span><span class="sxs-lookup"><span data-stu-id="60beb-111">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="60beb-112">Обновление агента будет выполняться в списке приоритетов ниже</span><span class="sxs-lookup"><span data-stu-id="60beb-112">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="60beb-113">Если для allowUpdateConfigurationOverride установлено значение true, конфигурация обновления, установленная клиентом, будет пропущена, и агент получит обновление при наличии следующей версии агента (приоритет 1).</span><span class="sxs-lookup"><span data-stu-id="60beb-113">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="60beb-114">Если задается отсрочка обновления, агент не будет обновлен до даты отсрочки обновления (приоритет 2).</span><span class="sxs-lookup"><span data-stu-id="60beb-114">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="60beb-115">Если установлено окно обновления, агент будет обновлен только в течение этого 24-часового дня (приоритет 3).</span><span class="sxs-lookup"><span data-stu-id="60beb-115">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="60beb-116">Если клиент не настроит допустимую конфигурацию средства обновления, агент получит обновление при наличии следующей версии агента.</span><span class="sxs-lookup"><span data-stu-id="60beb-116">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="60beb-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="60beb-117">Properties</span></span>

| <span data-ttu-id="60beb-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="60beb-118">Property</span></span>     | <span data-ttu-id="60beb-119">Тип</span><span class="sxs-lookup"><span data-stu-id="60beb-119">Type</span></span>        | <span data-ttu-id="60beb-120">Описание</span><span class="sxs-lookup"><span data-stu-id="60beb-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="60beb-121">allowUpdateConfigurationOverride</span><span class="sxs-lookup"><span data-stu-id="60beb-121">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="60beb-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="60beb-122">Boolean</span></span>|<span data-ttu-id="60beb-123">Указывает, будет ли пропущена конфигурация обновления, и агент получит обновление при наличии следующей версии агента.</span><span class="sxs-lookup"><span data-stu-id="60beb-123">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="60beb-124">deferUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="60beb-124">deferUpdateDateTime</span></span>|<span data-ttu-id="60beb-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60beb-125">DateTimeOffset</span></span>|<span data-ttu-id="60beb-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="60beb-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="60beb-128">updateWindow</span><span class="sxs-lookup"><span data-stu-id="60beb-128">updateWindow</span></span>|[<span data-ttu-id="60beb-129">updateWindow</span><span class="sxs-lookup"><span data-stu-id="60beb-129">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="60beb-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="60beb-130">JSON representation</span></span>

<span data-ttu-id="60beb-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="60beb-131">The following is a JSON representation of the resource.</span></span>

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


