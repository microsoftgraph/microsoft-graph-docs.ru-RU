---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c68fa195584c8d30cbe6a9b942a453b4f6a9218
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37357040"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="9b00f-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="9b00f-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="9b00f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="9b00f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b00f-105">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="9b00f-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="9b00f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9b00f-106">Properties</span></span>
|<span data-ttu-id="9b00f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9b00f-107">Property</span></span>|<span data-ttu-id="9b00f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9b00f-108">Type</span></span>|<span data-ttu-id="9b00f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9b00f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b00f-110">inventory</span><span class="sxs-lookup"><span data-stu-id="9b00f-110">inventory</span></span>|<span data-ttu-id="9b00f-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b00f-111">Boolean</span></span>|<span data-ttu-id="9b00f-112">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="9b00f-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="9b00f-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="9b00f-113">modernApps</span></span>|<span data-ttu-id="9b00f-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b00f-114">Boolean</span></span>|<span data-ttu-id="9b00f-115">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="9b00f-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="9b00f-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="9b00f-116">resourceAccess</span></span>|<span data-ttu-id="9b00f-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b00f-117">Boolean</span></span>|<span data-ttu-id="9b00f-118">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="9b00f-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="9b00f-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9b00f-119">deviceConfiguration</span></span>|<span data-ttu-id="9b00f-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b00f-120">Boolean</span></span>|<span data-ttu-id="9b00f-121">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="9b00f-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="9b00f-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="9b00f-122">compliancePolicy</span></span>|<span data-ttu-id="9b00f-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b00f-123">Boolean</span></span>|<span data-ttu-id="9b00f-124">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="9b00f-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="9b00f-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="9b00f-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="9b00f-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="9b00f-126">Boolean</span></span>|<span data-ttu-id="9b00f-127">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="9b00f-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b00f-128">Связи</span><span class="sxs-lookup"><span data-stu-id="9b00f-128">Relationships</span></span>
<span data-ttu-id="9b00f-129">Нет</span><span class="sxs-lookup"><span data-stu-id="9b00f-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b00f-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9b00f-130">JSON Representation</span></span>
<span data-ttu-id="9b00f-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9b00f-131">Here is a JSON representation of the resource.</span></span>
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




