---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed376bc616c26f1ad6e8a3ea06d3898c051e8d0b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148778"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="eae5c-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="eae5c-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="eae5c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eae5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eae5c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="eae5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eae5c-106">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="eae5c-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="eae5c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="eae5c-107">Properties</span></span>
|<span data-ttu-id="eae5c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="eae5c-108">Property</span></span>|<span data-ttu-id="eae5c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="eae5c-109">Type</span></span>|<span data-ttu-id="eae5c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="eae5c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eae5c-111">inventory</span><span class="sxs-lookup"><span data-stu-id="eae5c-111">inventory</span></span>|<span data-ttu-id="eae5c-112">Логический</span><span class="sxs-lookup"><span data-stu-id="eae5c-112">Boolean</span></span>|<span data-ttu-id="eae5c-113">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="eae5c-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="eae5c-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="eae5c-114">modernApps</span></span>|<span data-ttu-id="eae5c-115">Логический</span><span class="sxs-lookup"><span data-stu-id="eae5c-115">Boolean</span></span>|<span data-ttu-id="eae5c-116">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="eae5c-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="eae5c-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="eae5c-117">resourceAccess</span></span>|<span data-ttu-id="eae5c-118">Логический</span><span class="sxs-lookup"><span data-stu-id="eae5c-118">Boolean</span></span>|<span data-ttu-id="eae5c-119">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="eae5c-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="eae5c-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="eae5c-120">deviceConfiguration</span></span>|<span data-ttu-id="eae5c-121">Логический</span><span class="sxs-lookup"><span data-stu-id="eae5c-121">Boolean</span></span>|<span data-ttu-id="eae5c-122">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="eae5c-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="eae5c-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="eae5c-123">compliancePolicy</span></span>|<span data-ttu-id="eae5c-124">Логический</span><span class="sxs-lookup"><span data-stu-id="eae5c-124">Boolean</span></span>|<span data-ttu-id="eae5c-125">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="eae5c-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="eae5c-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="eae5c-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="eae5c-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="eae5c-127">Boolean</span></span>|<span data-ttu-id="eae5c-128">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="eae5c-128">Whether Windows Update for Business is managed by Intune</span></span>|
|<span data-ttu-id="eae5c-129">Ендпоинтпротектион</span><span class="sxs-lookup"><span data-stu-id="eae5c-129">endpointProtection</span></span>|<span data-ttu-id="eae5c-130">Логический</span><span class="sxs-lookup"><span data-stu-id="eae5c-130">Boolean</span></span>|<span data-ttu-id="eae5c-131">Управляет ли Intune Endpoint Protection</span><span class="sxs-lookup"><span data-stu-id="eae5c-131">Whether Endpoint Protection is managed by Intune</span></span>|
|<span data-ttu-id="eae5c-132">Оффицеаппс</span><span class="sxs-lookup"><span data-stu-id="eae5c-132">officeApps</span></span>|<span data-ttu-id="eae5c-133">Логический</span><span class="sxs-lookup"><span data-stu-id="eae5c-133">Boolean</span></span>|<span data-ttu-id="eae5c-134">Управляет ли Intune приложением Office</span><span class="sxs-lookup"><span data-stu-id="eae5c-134">Whether Office application is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="eae5c-135">Отношения</span><span class="sxs-lookup"><span data-stu-id="eae5c-135">Relationships</span></span>
<span data-ttu-id="eae5c-136">Нет</span><span class="sxs-lookup"><span data-stu-id="eae5c-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eae5c-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eae5c-137">JSON Representation</span></span>
<span data-ttu-id="eae5c-138">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eae5c-138">Here is a JSON representation of the resource.</span></span>
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




