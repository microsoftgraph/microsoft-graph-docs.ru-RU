---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: da8a32960b1a8e82f60161e329abcf68916b4f37
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43451274"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="27fd5-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="27fd5-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="27fd5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27fd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27fd5-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="27fd5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27fd5-106">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="27fd5-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="27fd5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="27fd5-107">Properties</span></span>
|<span data-ttu-id="27fd5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="27fd5-108">Property</span></span>|<span data-ttu-id="27fd5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="27fd5-109">Type</span></span>|<span data-ttu-id="27fd5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="27fd5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27fd5-111">inventory</span><span class="sxs-lookup"><span data-stu-id="27fd5-111">inventory</span></span>|<span data-ttu-id="27fd5-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="27fd5-112">Boolean</span></span>|<span data-ttu-id="27fd5-113">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="27fd5-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="27fd5-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="27fd5-114">modernApps</span></span>|<span data-ttu-id="27fd5-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="27fd5-115">Boolean</span></span>|<span data-ttu-id="27fd5-116">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="27fd5-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="27fd5-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="27fd5-117">resourceAccess</span></span>|<span data-ttu-id="27fd5-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="27fd5-118">Boolean</span></span>|<span data-ttu-id="27fd5-119">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="27fd5-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="27fd5-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="27fd5-120">deviceConfiguration</span></span>|<span data-ttu-id="27fd5-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="27fd5-121">Boolean</span></span>|<span data-ttu-id="27fd5-122">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="27fd5-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="27fd5-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="27fd5-123">compliancePolicy</span></span>|<span data-ttu-id="27fd5-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="27fd5-124">Boolean</span></span>|<span data-ttu-id="27fd5-125">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="27fd5-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="27fd5-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="27fd5-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="27fd5-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="27fd5-127">Boolean</span></span>|<span data-ttu-id="27fd5-128">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="27fd5-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="27fd5-129">Связи</span><span class="sxs-lookup"><span data-stu-id="27fd5-129">Relationships</span></span>
<span data-ttu-id="27fd5-130">Нет</span><span class="sxs-lookup"><span data-stu-id="27fd5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="27fd5-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27fd5-131">JSON Representation</span></span>
<span data-ttu-id="27fd5-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27fd5-132">Here is a JSON representation of the resource.</span></span>
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







