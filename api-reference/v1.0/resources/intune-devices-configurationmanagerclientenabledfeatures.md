---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c69e0ae9528a31ec7512348931e9a6eb0b1dd7b8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838943"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="35bf8-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="35bf8-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="35bf8-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="35bf8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35bf8-105">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="35bf8-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="35bf8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="35bf8-106">Properties</span></span>
|<span data-ttu-id="35bf8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="35bf8-107">Property</span></span>|<span data-ttu-id="35bf8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="35bf8-108">Type</span></span>|<span data-ttu-id="35bf8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="35bf8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35bf8-110">inventory</span><span class="sxs-lookup"><span data-stu-id="35bf8-110">inventory</span></span>|<span data-ttu-id="35bf8-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="35bf8-111">Boolean</span></span>|<span data-ttu-id="35bf8-112">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="35bf8-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="35bf8-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="35bf8-113">modernApps</span></span>|<span data-ttu-id="35bf8-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="35bf8-114">Boolean</span></span>|<span data-ttu-id="35bf8-115">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="35bf8-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="35bf8-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="35bf8-116">resourceAccess</span></span>|<span data-ttu-id="35bf8-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="35bf8-117">Boolean</span></span>|<span data-ttu-id="35bf8-118">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="35bf8-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="35bf8-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="35bf8-119">deviceConfiguration</span></span>|<span data-ttu-id="35bf8-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="35bf8-120">Boolean</span></span>|<span data-ttu-id="35bf8-121">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="35bf8-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="35bf8-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="35bf8-122">compliancePolicy</span></span>|<span data-ttu-id="35bf8-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="35bf8-123">Boolean</span></span>|<span data-ttu-id="35bf8-124">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="35bf8-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="35bf8-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="35bf8-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="35bf8-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="35bf8-126">Boolean</span></span>|<span data-ttu-id="35bf8-127">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="35bf8-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="35bf8-128">Связи</span><span class="sxs-lookup"><span data-stu-id="35bf8-128">Relationships</span></span>
<span data-ttu-id="35bf8-129">Нет</span><span class="sxs-lookup"><span data-stu-id="35bf8-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="35bf8-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35bf8-130">JSON Representation</span></span>
<span data-ttu-id="35bf8-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35bf8-131">Here is a JSON representation of the resource.</span></span>
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



