---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2dfae041f1aab4c4ea74490d372350c5c0c2087b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528685"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="4adee-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="4adee-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="4adee-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="4adee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4adee-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4adee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4adee-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4adee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4adee-107">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="4adee-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="4adee-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4adee-108">Properties</span></span>
|<span data-ttu-id="4adee-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4adee-109">Property</span></span>|<span data-ttu-id="4adee-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4adee-110">Type</span></span>|<span data-ttu-id="4adee-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4adee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4adee-112">inventory</span><span class="sxs-lookup"><span data-stu-id="4adee-112">inventory</span></span>|<span data-ttu-id="4adee-113">Логический</span><span class="sxs-lookup"><span data-stu-id="4adee-113">Boolean</span></span>|<span data-ttu-id="4adee-114">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="4adee-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="4adee-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="4adee-115">modernApps</span></span>|<span data-ttu-id="4adee-116">Логический</span><span class="sxs-lookup"><span data-stu-id="4adee-116">Boolean</span></span>|<span data-ttu-id="4adee-117">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="4adee-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="4adee-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="4adee-118">resourceAccess</span></span>|<span data-ttu-id="4adee-119">Логический</span><span class="sxs-lookup"><span data-stu-id="4adee-119">Boolean</span></span>|<span data-ttu-id="4adee-120">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="4adee-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="4adee-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4adee-121">deviceConfiguration</span></span>|<span data-ttu-id="4adee-122">Логический</span><span class="sxs-lookup"><span data-stu-id="4adee-122">Boolean</span></span>|<span data-ttu-id="4adee-123">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="4adee-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="4adee-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="4adee-124">compliancePolicy</span></span>|<span data-ttu-id="4adee-125">Логический</span><span class="sxs-lookup"><span data-stu-id="4adee-125">Boolean</span></span>|<span data-ttu-id="4adee-126">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="4adee-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="4adee-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="4adee-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="4adee-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="4adee-128">Boolean</span></span>|<span data-ttu-id="4adee-129">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="4adee-129">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="4adee-130">ендпоинтпротектион</span><span class="sxs-lookup"><span data-stu-id="4adee-130">endpointProtection</span></span>|<span data-ttu-id="4adee-131">Логический</span><span class="sxs-lookup"><span data-stu-id="4adee-131">Boolean</span></span>|<span data-ttu-id="4adee-132">Управляет ли Intune Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="4adee-132">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="4adee-133">оффицеаппс</span><span class="sxs-lookup"><span data-stu-id="4adee-133">officeApps</span></span>|<span data-ttu-id="4adee-134">Логический</span><span class="sxs-lookup"><span data-stu-id="4adee-134">Boolean</span></span>|<span data-ttu-id="4adee-135">Управляет ли Intune приложением Office</span><span class="sxs-lookup"><span data-stu-id="4adee-135">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="4adee-136">Связи</span><span class="sxs-lookup"><span data-stu-id="4adee-136">Relationships</span></span>
<span data-ttu-id="4adee-137">Нет</span><span class="sxs-lookup"><span data-stu-id="4adee-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4adee-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4adee-138">JSON Representation</span></span>
<span data-ttu-id="4adee-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4adee-139">Here is a JSON representation of the resource.</span></span>
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



