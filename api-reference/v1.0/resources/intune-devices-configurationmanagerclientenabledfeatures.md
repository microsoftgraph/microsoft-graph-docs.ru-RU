---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 520b21445d4c5a61755ddc78c65b9999a7e45ff0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027498"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="195f2-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="195f2-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="195f2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="195f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="195f2-105">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="195f2-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="195f2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="195f2-106">Properties</span></span>
|<span data-ttu-id="195f2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="195f2-107">Property</span></span>|<span data-ttu-id="195f2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="195f2-108">Type</span></span>|<span data-ttu-id="195f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="195f2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="195f2-110">inventory</span><span class="sxs-lookup"><span data-stu-id="195f2-110">inventory</span></span>|<span data-ttu-id="195f2-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="195f2-111">Boolean</span></span>|<span data-ttu-id="195f2-112">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="195f2-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="195f2-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="195f2-113">modernApps</span></span>|<span data-ttu-id="195f2-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="195f2-114">Boolean</span></span>|<span data-ttu-id="195f2-115">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="195f2-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="195f2-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="195f2-116">resourceAccess</span></span>|<span data-ttu-id="195f2-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="195f2-117">Boolean</span></span>|<span data-ttu-id="195f2-118">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="195f2-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="195f2-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="195f2-119">deviceConfiguration</span></span>|<span data-ttu-id="195f2-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="195f2-120">Boolean</span></span>|<span data-ttu-id="195f2-121">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="195f2-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="195f2-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="195f2-122">compliancePolicy</span></span>|<span data-ttu-id="195f2-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="195f2-123">Boolean</span></span>|<span data-ttu-id="195f2-124">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="195f2-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="195f2-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="195f2-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="195f2-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="195f2-126">Boolean</span></span>|<span data-ttu-id="195f2-127">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="195f2-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="195f2-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="195f2-128">Relationships</span></span>
<span data-ttu-id="195f2-129">Нет</span><span class="sxs-lookup"><span data-stu-id="195f2-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="195f2-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="195f2-130">JSON Representation</span></span>
<span data-ttu-id="195f2-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="195f2-131">Here is a JSON representation of the resource.</span></span>
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



