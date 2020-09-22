---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 317378e58c870e77140ae961925aeb59a001daff
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060645"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="750e7-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="750e7-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="750e7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="750e7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="750e7-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="750e7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="750e7-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="750e7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="750e7-107">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="750e7-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="750e7-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="750e7-108">Properties</span></span>
|<span data-ttu-id="750e7-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="750e7-109">Property</span></span>|<span data-ttu-id="750e7-110">Тип</span><span class="sxs-lookup"><span data-stu-id="750e7-110">Type</span></span>|<span data-ttu-id="750e7-111">Описание</span><span class="sxs-lookup"><span data-stu-id="750e7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="750e7-112">inventory</span><span class="sxs-lookup"><span data-stu-id="750e7-112">inventory</span></span>|<span data-ttu-id="750e7-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="750e7-113">Boolean</span></span>|<span data-ttu-id="750e7-114">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="750e7-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="750e7-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="750e7-115">modernApps</span></span>|<span data-ttu-id="750e7-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="750e7-116">Boolean</span></span>|<span data-ttu-id="750e7-117">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="750e7-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="750e7-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="750e7-118">resourceAccess</span></span>|<span data-ttu-id="750e7-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="750e7-119">Boolean</span></span>|<span data-ttu-id="750e7-120">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="750e7-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="750e7-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="750e7-121">deviceConfiguration</span></span>|<span data-ttu-id="750e7-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="750e7-122">Boolean</span></span>|<span data-ttu-id="750e7-123">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="750e7-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="750e7-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="750e7-124">compliancePolicy</span></span>|<span data-ttu-id="750e7-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="750e7-125">Boolean</span></span>|<span data-ttu-id="750e7-126">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="750e7-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="750e7-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="750e7-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="750e7-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="750e7-128">Boolean</span></span>|<span data-ttu-id="750e7-129">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="750e7-129">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="750e7-130">ендпоинтпротектион</span><span class="sxs-lookup"><span data-stu-id="750e7-130">endpointProtection</span></span>|<span data-ttu-id="750e7-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="750e7-131">Boolean</span></span>|<span data-ttu-id="750e7-132">Управляет ли Intune Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="750e7-132">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="750e7-133">оффицеаппс</span><span class="sxs-lookup"><span data-stu-id="750e7-133">officeApps</span></span>|<span data-ttu-id="750e7-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="750e7-134">Boolean</span></span>|<span data-ttu-id="750e7-135">Управляет ли Intune приложением Office</span><span class="sxs-lookup"><span data-stu-id="750e7-135">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="750e7-136">Связи</span><span class="sxs-lookup"><span data-stu-id="750e7-136">Relationships</span></span>
<span data-ttu-id="750e7-137">Нет</span><span class="sxs-lookup"><span data-stu-id="750e7-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="750e7-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="750e7-138">JSON Representation</span></span>
<span data-ttu-id="750e7-139">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="750e7-139">Here is a JSON representation of the resource.</span></span>
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






