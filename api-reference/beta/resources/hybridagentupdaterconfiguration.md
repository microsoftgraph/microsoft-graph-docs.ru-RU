---
title: Тип ресурса Хибридажентупдатерконфигуратион
description: Тип ресурса Хибридажентупдатерконфигуратион.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: cf948d8404a4887770477b8e4b3e7812bd8516cc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013589"
---
# <a name="hybridagentupdaterconfiguration-resource-type"></a><span data-ttu-id="40774-103">Тип ресурса Хибридажентупдатерконфигуратион</span><span class="sxs-lookup"><span data-stu-id="40774-103">hybridAgentUpdaterConfiguration resource type</span></span>

<span data-ttu-id="40774-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40774-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="40774-105">Администратор клиента может настраивать для каждого Онпремисеспублишингпрофиле периода времени, в течение которого агенты могут получать обновления или закладывать обновления для агентов.</span><span class="sxs-lookup"><span data-stu-id="40774-105">A tenant admin can configure for each onPremisesPublishingProfile the time window during which agents can receive updates or defer updates to the agents.</span></span> <span data-ttu-id="40774-106">Хибридажентупдатерконфигуратион, заданный для Онпремисеспублишингпрофиле, можно применить ко всем агентам в пределах этого Онпремисеспублишингпрофиле.</span><span class="sxs-lookup"><span data-stu-id="40774-106">The hybridAgentUpdaterConfiguration specified for an onPremisesPublishingProfile is applicable to all the agents within that onPremisesPublishingProfile.</span></span>

<span data-ttu-id="40774-107">Например, для агентов в Онпремисеспублишингпрофиле типа "подготовка" эти действия могут быть выполнены следующим образом.</span><span class="sxs-lookup"><span data-stu-id="40774-107">For example, for the agents in onPremisesPublishingProfile of type "provisioning" the steps could be as below.</span></span>

1) <span data-ttu-id="40774-108">Администратор клиента может настроить, чтобы не получалось никаких обновлений агентов подготовки в течение следующих n дней.</span><span class="sxs-lookup"><span data-stu-id="40774-108">Tenant administrator can configure to not receive any updates to the Provisioning agents for the next n days.</span></span>
2) <span data-ttu-id="40774-109">Администратор клиента может настроить окно обновления (время начала и время окончания), в течение которого агенты могут реЦиве обновления.</span><span class="sxs-lookup"><span data-stu-id="40774-109">Tenant administrator can configure an update window(start and end time) during which the agents can recive updates.</span></span>
3) <span data-ttu-id="40774-110">Администратор клиента может включить Алловупдатеконфигуратионоверриде, который переопределяет конфигутратион обновления для агентов подготовки и аловс их для получения следующего доступного обновления.</span><span class="sxs-lookup"><span data-stu-id="40774-110">Tenant administrator can enable allowUpdateConfigurationOverride which overrides the updater configutration for Provisioning agents and alows them to receive the next available update.</span></span>

<span data-ttu-id="40774-111">Сведения о времени и времени, указанные в конфигурации обновления, будут преобразованы в локальный часовой пояс, указанный агентом во время евалуватион.</span><span class="sxs-lookup"><span data-stu-id="40774-111">The DateTime/Time information specified in the updater configuration will be converted to the local timezone reported by the agent during evaluvation.</span></span>

<span data-ttu-id="40774-112">Обновленный агент будет соответствовать списку приоритетов, приведенному ниже.</span><span class="sxs-lookup"><span data-stu-id="40774-112">The update of the agent will follow the below priority list</span></span>

1) <span data-ttu-id="40774-113">Если для Алловупдатеконфигуратионоверриде задано значение true, набор конфигураций обновлений, заданный клиентом, будет пропущен и агент будет получать обновление при доступности следующей версии агента (приоритет 1).</span><span class="sxs-lookup"><span data-stu-id="40774-113">If allowUpdateConfigurationOverride is set to true the updater configuration set by the tenant will be skipped and the agent will receive an update when the next version of the agent is available (priority 1).</span></span>
2) <span data-ttu-id="40774-114">Если установлено отложенное обновление, агент не будет обновляться до даты отсрочки обновления (приоритет 2).</span><span class="sxs-lookup"><span data-stu-id="40774-114">If the defer update is set, the agent will not be updated until the defer update date time (priority 2).</span></span>
3) <span data-ttu-id="40774-115">Если окно обновления установлено, агент будет обновляться только в течение этого периода времени в 24-часовом дне (приоритет 3).</span><span class="sxs-lookup"><span data-stu-id="40774-115">If the update window is set, the agent will be updated only during that time window in a 24 hour day (priority 3).</span></span>
4) <span data-ttu-id="40774-116">Если клиент не устанавливает действительную конфигурацию обновлений, агент получит обновление, когда будет доступна следующая версия агента.</span><span class="sxs-lookup"><span data-stu-id="40774-116">If no valid updater configuration is set by the tenant, the agent will receive an update when the next version of the agent is available</span></span>

## <a name="properties"></a><span data-ttu-id="40774-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="40774-117">Properties</span></span>

| <span data-ttu-id="40774-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="40774-118">Property</span></span>     | <span data-ttu-id="40774-119">Тип</span><span class="sxs-lookup"><span data-stu-id="40774-119">Type</span></span>        | <span data-ttu-id="40774-120">Описание</span><span class="sxs-lookup"><span data-stu-id="40774-120">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="40774-121">алловупдатеконфигуратионоверриде</span><span class="sxs-lookup"><span data-stu-id="40774-121">allowUpdateConfigurationOverride</span></span>|<span data-ttu-id="40774-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="40774-122">Boolean</span></span>|<span data-ttu-id="40774-123">Указывает, будет ли пропущена Конфигурация обновления, и агент будет получать обновление при наличии следующей версии агента.</span><span class="sxs-lookup"><span data-stu-id="40774-123">Indicates if updater configuration will be skipped and the agent will receive an update when the next version of the agent is available.</span></span>|
|<span data-ttu-id="40774-124">деферупдатедатетиме</span><span class="sxs-lookup"><span data-stu-id="40774-124">deferUpdateDateTime</span></span>|<span data-ttu-id="40774-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40774-125">DateTimeOffset</span></span>|<span data-ttu-id="40774-p102">Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда используется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC выглядит так: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="40774-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="40774-128">упдатевиндов</span><span class="sxs-lookup"><span data-stu-id="40774-128">updateWindow</span></span>|[<span data-ttu-id="40774-129">упдатевиндов</span><span class="sxs-lookup"><span data-stu-id="40774-129">updateWindow</span></span>](updatewindow.md)||

## <a name="json-representation"></a><span data-ttu-id="40774-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40774-130">JSON representation</span></span>

<span data-ttu-id="40774-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40774-131">The following is a JSON representation of the resource.</span></span>

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


