---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7975130bb047e097ea0d52a4ce770fb35e4efa32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425906"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="3e0b4-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="3e0b4-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="3e0b4-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e0b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3e0b4-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e0b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e0b4-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3e0b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e0b4-107">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="3e0b4-107">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="3e0b4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e0b4-108">Properties</span></span>
|<span data-ttu-id="3e0b4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e0b4-109">Property</span></span>|<span data-ttu-id="3e0b4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e0b4-110">Type</span></span>|<span data-ttu-id="3e0b4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e0b4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e0b4-112">inventory</span><span class="sxs-lookup"><span data-stu-id="3e0b4-112">inventory</span></span>|<span data-ttu-id="3e0b4-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e0b4-113">Boolean</span></span>|<span data-ttu-id="3e0b4-114">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="3e0b4-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="3e0b4-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="3e0b4-115">modernApps</span></span>|<span data-ttu-id="3e0b4-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e0b4-116">Boolean</span></span>|<span data-ttu-id="3e0b4-117">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="3e0b4-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="3e0b4-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="3e0b4-118">resourceAccess</span></span>|<span data-ttu-id="3e0b4-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e0b4-119">Boolean</span></span>|<span data-ttu-id="3e0b4-120">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="3e0b4-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="3e0b4-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3e0b4-121">deviceConfiguration</span></span>|<span data-ttu-id="3e0b4-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e0b4-122">Boolean</span></span>|<span data-ttu-id="3e0b4-123">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="3e0b4-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="3e0b4-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3e0b4-124">compliancePolicy</span></span>|<span data-ttu-id="3e0b4-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e0b4-125">Boolean</span></span>|<span data-ttu-id="3e0b4-126">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="3e0b4-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="3e0b4-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="3e0b4-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="3e0b4-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="3e0b4-128">Boolean</span></span>|<span data-ttu-id="3e0b4-129">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="3e0b4-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e0b4-130">Связи</span><span class="sxs-lookup"><span data-stu-id="3e0b4-130">Relationships</span></span>
<span data-ttu-id="3e0b4-131">Нет</span><span class="sxs-lookup"><span data-stu-id="3e0b4-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e0b4-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e0b4-132">JSON Representation</span></span>
<span data-ttu-id="3e0b4-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e0b4-133">Here is a JSON representation of the resource.</span></span>
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




