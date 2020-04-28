---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 189751d12f7220dcfa4e3e6985c3913bb7ae0e32
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465062"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="f91a6-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="f91a6-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="f91a6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f91a6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f91a6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f91a6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f91a6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f91a6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f91a6-107">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="f91a6-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="f91a6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f91a6-108">Properties</span></span>
|<span data-ttu-id="f91a6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f91a6-109">Property</span></span>|<span data-ttu-id="f91a6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f91a6-110">Type</span></span>|<span data-ttu-id="f91a6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f91a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f91a6-112">inventory</span><span class="sxs-lookup"><span data-stu-id="f91a6-112">inventory</span></span>|<span data-ttu-id="f91a6-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91a6-113">Boolean</span></span>|<span data-ttu-id="f91a6-114">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="f91a6-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="f91a6-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="f91a6-115">modernApps</span></span>|<span data-ttu-id="f91a6-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91a6-116">Boolean</span></span>|<span data-ttu-id="f91a6-117">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="f91a6-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="f91a6-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="f91a6-118">resourceAccess</span></span>|<span data-ttu-id="f91a6-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91a6-119">Boolean</span></span>|<span data-ttu-id="f91a6-120">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="f91a6-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="f91a6-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f91a6-121">deviceConfiguration</span></span>|<span data-ttu-id="f91a6-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91a6-122">Boolean</span></span>|<span data-ttu-id="f91a6-123">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="f91a6-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="f91a6-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="f91a6-124">compliancePolicy</span></span>|<span data-ttu-id="f91a6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91a6-125">Boolean</span></span>|<span data-ttu-id="f91a6-126">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="f91a6-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="f91a6-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="f91a6-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="f91a6-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91a6-128">Boolean</span></span>|<span data-ttu-id="f91a6-129">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="f91a6-129">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="f91a6-130">ендпоинтпротектион</span><span class="sxs-lookup"><span data-stu-id="f91a6-130">endpointProtection</span></span>|<span data-ttu-id="f91a6-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91a6-131">Boolean</span></span>|<span data-ttu-id="f91a6-132">Управляет ли Intune Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="f91a6-132">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="f91a6-133">оффицеаппс</span><span class="sxs-lookup"><span data-stu-id="f91a6-133">officeApps</span></span>|<span data-ttu-id="f91a6-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="f91a6-134">Boolean</span></span>|<span data-ttu-id="f91a6-135">Управляет ли Intune приложением Office</span><span class="sxs-lookup"><span data-stu-id="f91a6-135">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="f91a6-136">Связи</span><span class="sxs-lookup"><span data-stu-id="f91a6-136">Relationships</span></span>
<span data-ttu-id="f91a6-137">Нет</span><span class="sxs-lookup"><span data-stu-id="f91a6-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f91a6-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f91a6-138">JSON Representation</span></span>
<span data-ttu-id="f91a6-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f91a6-139">Here is a JSON representation of the resource.</span></span>
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



