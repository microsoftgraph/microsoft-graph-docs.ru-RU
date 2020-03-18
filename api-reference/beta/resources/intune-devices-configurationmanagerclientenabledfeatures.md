---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ce366adec1bcab58df761a6a271a45fbd0510c03
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785072"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="becb2-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="becb2-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="becb2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="becb2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="becb2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="becb2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="becb2-106">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="becb2-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="becb2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="becb2-107">Properties</span></span>
|<span data-ttu-id="becb2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="becb2-108">Property</span></span>|<span data-ttu-id="becb2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="becb2-109">Type</span></span>|<span data-ttu-id="becb2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="becb2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="becb2-111">inventory</span><span class="sxs-lookup"><span data-stu-id="becb2-111">inventory</span></span>|<span data-ttu-id="becb2-112">Логический</span><span class="sxs-lookup"><span data-stu-id="becb2-112">Boolean</span></span>|<span data-ttu-id="becb2-113">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="becb2-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="becb2-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="becb2-114">modernApps</span></span>|<span data-ttu-id="becb2-115">Логический</span><span class="sxs-lookup"><span data-stu-id="becb2-115">Boolean</span></span>|<span data-ttu-id="becb2-116">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="becb2-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="becb2-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="becb2-117">resourceAccess</span></span>|<span data-ttu-id="becb2-118">Логический</span><span class="sxs-lookup"><span data-stu-id="becb2-118">Boolean</span></span>|<span data-ttu-id="becb2-119">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="becb2-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="becb2-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="becb2-120">deviceConfiguration</span></span>|<span data-ttu-id="becb2-121">Логический</span><span class="sxs-lookup"><span data-stu-id="becb2-121">Boolean</span></span>|<span data-ttu-id="becb2-122">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="becb2-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="becb2-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="becb2-123">compliancePolicy</span></span>|<span data-ttu-id="becb2-124">Логический</span><span class="sxs-lookup"><span data-stu-id="becb2-124">Boolean</span></span>|<span data-ttu-id="becb2-125">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="becb2-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="becb2-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="becb2-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="becb2-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="becb2-127">Boolean</span></span>|<span data-ttu-id="becb2-128">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="becb2-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="becb2-129">ендпоинтпротектион</span><span class="sxs-lookup"><span data-stu-id="becb2-129">endpointProtection</span></span>|<span data-ttu-id="becb2-130">Логический</span><span class="sxs-lookup"><span data-stu-id="becb2-130">Boolean</span></span>|<span data-ttu-id="becb2-131">Управляет ли Intune Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="becb2-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="becb2-132">оффицеаппс</span><span class="sxs-lookup"><span data-stu-id="becb2-132">officeApps</span></span>|<span data-ttu-id="becb2-133">Логический</span><span class="sxs-lookup"><span data-stu-id="becb2-133">Boolean</span></span>|<span data-ttu-id="becb2-134">Управляет ли Intune приложением Office</span><span class="sxs-lookup"><span data-stu-id="becb2-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="becb2-135">Связи</span><span class="sxs-lookup"><span data-stu-id="becb2-135">Relationships</span></span>
<span data-ttu-id="becb2-136">Нет</span><span class="sxs-lookup"><span data-stu-id="becb2-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="becb2-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="becb2-137">JSON Representation</span></span>
<span data-ttu-id="becb2-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="becb2-138">Here is a JSON representation of the resource.</span></span>
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



