---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91ffd0180660b33e9ead5210f9b23870af18e29a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467311"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="2184e-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="2184e-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="2184e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2184e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2184e-105">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="2184e-105">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="2184e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2184e-106">Properties</span></span>
|<span data-ttu-id="2184e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2184e-107">Property</span></span>|<span data-ttu-id="2184e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2184e-108">Type</span></span>|<span data-ttu-id="2184e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2184e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2184e-110">inventory</span><span class="sxs-lookup"><span data-stu-id="2184e-110">inventory</span></span>|<span data-ttu-id="2184e-111">Логический</span><span class="sxs-lookup"><span data-stu-id="2184e-111">Boolean</span></span>|<span data-ttu-id="2184e-112">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="2184e-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="2184e-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="2184e-113">modernApps</span></span>|<span data-ttu-id="2184e-114">Логический</span><span class="sxs-lookup"><span data-stu-id="2184e-114">Boolean</span></span>|<span data-ttu-id="2184e-115">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="2184e-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="2184e-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="2184e-116">resourceAccess</span></span>|<span data-ttu-id="2184e-117">Логический</span><span class="sxs-lookup"><span data-stu-id="2184e-117">Boolean</span></span>|<span data-ttu-id="2184e-118">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="2184e-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="2184e-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="2184e-119">deviceConfiguration</span></span>|<span data-ttu-id="2184e-120">Логический</span><span class="sxs-lookup"><span data-stu-id="2184e-120">Boolean</span></span>|<span data-ttu-id="2184e-121">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="2184e-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="2184e-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="2184e-122">compliancePolicy</span></span>|<span data-ttu-id="2184e-123">Логический</span><span class="sxs-lookup"><span data-stu-id="2184e-123">Boolean</span></span>|<span data-ttu-id="2184e-124">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="2184e-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="2184e-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="2184e-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="2184e-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="2184e-126">Boolean</span></span>|<span data-ttu-id="2184e-127">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="2184e-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="2184e-128">Отношения</span><span class="sxs-lookup"><span data-stu-id="2184e-128">Relationships</span></span>
<span data-ttu-id="2184e-129">Нет</span><span class="sxs-lookup"><span data-stu-id="2184e-129">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2184e-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2184e-130">JSON Representation</span></span>
<span data-ttu-id="2184e-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2184e-131">Here is a JSON representation of the resource.</span></span>
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



