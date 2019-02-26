---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264423"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="924f0-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="924f0-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="924f0-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="924f0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="924f0-105">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="924f0-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="924f0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="924f0-106">Properties</span></span>
|<span data-ttu-id="924f0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="924f0-107">Property</span></span>|<span data-ttu-id="924f0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="924f0-108">Type</span></span>|<span data-ttu-id="924f0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="924f0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="924f0-110">inventory</span><span class="sxs-lookup"><span data-stu-id="924f0-110">inventory</span></span>|<span data-ttu-id="924f0-111">Логический</span><span class="sxs-lookup"><span data-stu-id="924f0-111">Boolean</span></span>|<span data-ttu-id="924f0-112">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="924f0-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="924f0-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="924f0-113">modernApps</span></span>|<span data-ttu-id="924f0-114">Логический</span><span class="sxs-lookup"><span data-stu-id="924f0-114">Boolean</span></span>|<span data-ttu-id="924f0-115">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="924f0-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="924f0-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="924f0-116">resourceAccess</span></span>|<span data-ttu-id="924f0-117">Логический</span><span class="sxs-lookup"><span data-stu-id="924f0-117">Boolean</span></span>|<span data-ttu-id="924f0-118">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="924f0-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="924f0-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="924f0-119">deviceConfiguration</span></span>|<span data-ttu-id="924f0-120">Логический</span><span class="sxs-lookup"><span data-stu-id="924f0-120">Boolean</span></span>|<span data-ttu-id="924f0-121">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="924f0-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="924f0-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="924f0-122">compliancePolicy</span></span>|<span data-ttu-id="924f0-123">Логический</span><span class="sxs-lookup"><span data-stu-id="924f0-123">Boolean</span></span>|<span data-ttu-id="924f0-124">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="924f0-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="924f0-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="924f0-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="924f0-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="924f0-126">Boolean</span></span>|<span data-ttu-id="924f0-127">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="924f0-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="924f0-128">Связи</span><span class="sxs-lookup"><span data-stu-id="924f0-128">Relationships</span></span>
<span data-ttu-id="924f0-129">Нет</span><span class="sxs-lookup"><span data-stu-id="924f0-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="924f0-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="924f0-130">JSON Representation</span></span>
<span data-ttu-id="924f0-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="924f0-131">Here is a JSON representation of the resource.</span></span>
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
  "windowsUpdateForBusiness": true
}
```



