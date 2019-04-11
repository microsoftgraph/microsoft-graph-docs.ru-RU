---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a90b7f0009b4d9bd617b781338ceee3de2f432c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787927"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="5ac80-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="5ac80-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="5ac80-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5ac80-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ac80-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ac80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ac80-106">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="5ac80-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="5ac80-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ac80-107">Properties</span></span>
|<span data-ttu-id="5ac80-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ac80-108">Property</span></span>|<span data-ttu-id="5ac80-109">Тип</span><span class="sxs-lookup"><span data-stu-id="5ac80-109">Type</span></span>|<span data-ttu-id="5ac80-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5ac80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ac80-111">inventory</span><span class="sxs-lookup"><span data-stu-id="5ac80-111">inventory</span></span>|<span data-ttu-id="5ac80-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ac80-112">Boolean</span></span>|<span data-ttu-id="5ac80-113">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="5ac80-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="5ac80-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="5ac80-114">modernApps</span></span>|<span data-ttu-id="5ac80-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ac80-115">Boolean</span></span>|<span data-ttu-id="5ac80-116">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="5ac80-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="5ac80-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="5ac80-117">resourceAccess</span></span>|<span data-ttu-id="5ac80-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ac80-118">Boolean</span></span>|<span data-ttu-id="5ac80-119">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="5ac80-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="5ac80-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="5ac80-120">deviceConfiguration</span></span>|<span data-ttu-id="5ac80-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ac80-121">Boolean</span></span>|<span data-ttu-id="5ac80-122">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="5ac80-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="5ac80-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="5ac80-123">compliancePolicy</span></span>|<span data-ttu-id="5ac80-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ac80-124">Boolean</span></span>|<span data-ttu-id="5ac80-125">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="5ac80-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="5ac80-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="5ac80-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="5ac80-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ac80-127">Boolean</span></span>|<span data-ttu-id="5ac80-128">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="5ac80-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="5ac80-129">Ендпоинтпротектион</span><span class="sxs-lookup"><span data-stu-id="5ac80-129">endpointProtection</span></span>|<span data-ttu-id="5ac80-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ac80-130">Boolean</span></span>|<span data-ttu-id="5ac80-131">Управляет ли Intune Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="5ac80-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="5ac80-132">Оффицеаппс</span><span class="sxs-lookup"><span data-stu-id="5ac80-132">officeApps</span></span>|<span data-ttu-id="5ac80-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ac80-133">Boolean</span></span>|<span data-ttu-id="5ac80-134">Управляет ли Intune приложением Office</span><span class="sxs-lookup"><span data-stu-id="5ac80-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ac80-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="5ac80-135">Relationships</span></span>
<span data-ttu-id="5ac80-136">Нет</span><span class="sxs-lookup"><span data-stu-id="5ac80-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ac80-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ac80-137">JSON Representation</span></span>
<span data-ttu-id="5ac80-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ac80-138">Here is a JSON representation of the resource.</span></span>
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





