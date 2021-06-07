---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d9d7cab901b78eb980a3617735e94a892f11d634
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751701"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="78d80-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="78d80-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="78d80-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78d80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78d80-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78d80-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78d80-106">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="78d80-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="78d80-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="78d80-107">Properties</span></span>
|<span data-ttu-id="78d80-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="78d80-108">Property</span></span>|<span data-ttu-id="78d80-109">Тип</span><span class="sxs-lookup"><span data-stu-id="78d80-109">Type</span></span>|<span data-ttu-id="78d80-110">Описание</span><span class="sxs-lookup"><span data-stu-id="78d80-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78d80-111">inventory</span><span class="sxs-lookup"><span data-stu-id="78d80-111">inventory</span></span>|<span data-ttu-id="78d80-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d80-112">Boolean</span></span>|<span data-ttu-id="78d80-113">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="78d80-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="78d80-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="78d80-114">modernApps</span></span>|<span data-ttu-id="78d80-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d80-115">Boolean</span></span>|<span data-ttu-id="78d80-116">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="78d80-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="78d80-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="78d80-117">resourceAccess</span></span>|<span data-ttu-id="78d80-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d80-118">Boolean</span></span>|<span data-ttu-id="78d80-119">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="78d80-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="78d80-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="78d80-120">deviceConfiguration</span></span>|<span data-ttu-id="78d80-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d80-121">Boolean</span></span>|<span data-ttu-id="78d80-122">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="78d80-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="78d80-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="78d80-123">compliancePolicy</span></span>|<span data-ttu-id="78d80-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d80-124">Boolean</span></span>|<span data-ttu-id="78d80-125">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="78d80-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="78d80-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="78d80-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="78d80-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="78d80-127">Boolean</span></span>|<span data-ttu-id="78d80-128">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="78d80-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="78d80-129">Отношения</span><span class="sxs-lookup"><span data-stu-id="78d80-129">Relationships</span></span>
<span data-ttu-id="78d80-130">Нет</span><span class="sxs-lookup"><span data-stu-id="78d80-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78d80-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78d80-131">JSON Representation</span></span>
<span data-ttu-id="78d80-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78d80-132">Here is a JSON representation of the resource.</span></span>
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




