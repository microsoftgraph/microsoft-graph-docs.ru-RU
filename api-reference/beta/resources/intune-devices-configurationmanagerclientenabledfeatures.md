---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 37c098910ec532a1ab23ae8464c03e43cf7a9e29
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943041"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="4c15f-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4c15f-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="4c15f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4c15f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c15f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4c15f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c15f-106">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="4c15f-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="4c15f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4c15f-107">Properties</span></span>
|<span data-ttu-id="4c15f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4c15f-108">Property</span></span>|<span data-ttu-id="4c15f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4c15f-109">Type</span></span>|<span data-ttu-id="4c15f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4c15f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c15f-111">inventory</span><span class="sxs-lookup"><span data-stu-id="4c15f-111">inventory</span></span>|<span data-ttu-id="4c15f-112">Логический</span><span class="sxs-lookup"><span data-stu-id="4c15f-112">Boolean</span></span>|<span data-ttu-id="4c15f-113">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="4c15f-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="4c15f-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="4c15f-114">modernApps</span></span>|<span data-ttu-id="4c15f-115">Логический</span><span class="sxs-lookup"><span data-stu-id="4c15f-115">Boolean</span></span>|<span data-ttu-id="4c15f-116">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="4c15f-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="4c15f-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="4c15f-117">resourceAccess</span></span>|<span data-ttu-id="4c15f-118">Логический</span><span class="sxs-lookup"><span data-stu-id="4c15f-118">Boolean</span></span>|<span data-ttu-id="4c15f-119">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="4c15f-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="4c15f-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c15f-120">deviceConfiguration</span></span>|<span data-ttu-id="4c15f-121">Логический</span><span class="sxs-lookup"><span data-stu-id="4c15f-121">Boolean</span></span>|<span data-ttu-id="4c15f-122">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="4c15f-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="4c15f-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4c15f-123">compliancePolicy</span></span>|<span data-ttu-id="4c15f-124">Логический</span><span class="sxs-lookup"><span data-stu-id="4c15f-124">Boolean</span></span>|<span data-ttu-id="4c15f-125">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="4c15f-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="4c15f-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="4c15f-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="4c15f-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c15f-127">Boolean</span></span>|<span data-ttu-id="4c15f-128">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="4c15f-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="4c15f-129">Ендпоинтпротектион</span><span class="sxs-lookup"><span data-stu-id="4c15f-129">endpointProtection</span></span>|<span data-ttu-id="4c15f-130">Логический</span><span class="sxs-lookup"><span data-stu-id="4c15f-130">Boolean</span></span>|<span data-ttu-id="4c15f-131">Управляет ли Intune Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="4c15f-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="4c15f-132">Оффицеаппс</span><span class="sxs-lookup"><span data-stu-id="4c15f-132">officeApps</span></span>|<span data-ttu-id="4c15f-133">Логический</span><span class="sxs-lookup"><span data-stu-id="4c15f-133">Boolean</span></span>|<span data-ttu-id="4c15f-134">Управляет ли Intune приложением Office</span><span class="sxs-lookup"><span data-stu-id="4c15f-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c15f-135">Связи</span><span class="sxs-lookup"><span data-stu-id="4c15f-135">Relationships</span></span>
<span data-ttu-id="4c15f-136">Нет</span><span class="sxs-lookup"><span data-stu-id="4c15f-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c15f-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4c15f-137">JSON Representation</span></span>
<span data-ttu-id="4c15f-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4c15f-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientEnabledFeatures",
  "inventory": true,
  "modernApps": true,
  "resourceAccess": true,
  "deviceConfiguration": true,
  "compliancePolicy": true,
  "windowsUpdateForBusiness": true,
  "endpointProtection": true,
  "officeApps": true
}
```




