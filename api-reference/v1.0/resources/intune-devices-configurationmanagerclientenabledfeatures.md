---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e8622f6f1772948295f9389cf97aef0b6f260e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533311"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="ecad7-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="ecad7-103">configurationManagerClientEnabledFeatures resource type</span></span>

<span data-ttu-id="ecad7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecad7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ecad7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ecad7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecad7-106">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="ecad7-106">configuration Manager client enabled features</span></span>

## <a name="properties"></a><span data-ttu-id="ecad7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ecad7-107">Properties</span></span>
|<span data-ttu-id="ecad7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ecad7-108">Property</span></span>|<span data-ttu-id="ecad7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ecad7-109">Type</span></span>|<span data-ttu-id="ecad7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ecad7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecad7-111">inventory</span><span class="sxs-lookup"><span data-stu-id="ecad7-111">inventory</span></span>|<span data-ttu-id="ecad7-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecad7-112">Boolean</span></span>|<span data-ttu-id="ecad7-113">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="ecad7-113">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="ecad7-114">modernApps</span><span class="sxs-lookup"><span data-stu-id="ecad7-114">modernApps</span></span>|<span data-ttu-id="ecad7-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecad7-115">Boolean</span></span>|<span data-ttu-id="ecad7-116">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="ecad7-116">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="ecad7-117">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="ecad7-117">resourceAccess</span></span>|<span data-ttu-id="ecad7-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecad7-118">Boolean</span></span>|<span data-ttu-id="ecad7-119">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="ecad7-119">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="ecad7-120">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="ecad7-120">deviceConfiguration</span></span>|<span data-ttu-id="ecad7-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecad7-121">Boolean</span></span>|<span data-ttu-id="ecad7-122">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="ecad7-122">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="ecad7-123">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="ecad7-123">compliancePolicy</span></span>|<span data-ttu-id="ecad7-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecad7-124">Boolean</span></span>|<span data-ttu-id="ecad7-125">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="ecad7-125">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="ecad7-126">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="ecad7-126">windowsUpdateForBusiness</span></span>|<span data-ttu-id="ecad7-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="ecad7-127">Boolean</span></span>|<span data-ttu-id="ecad7-128">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="ecad7-128">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="ecad7-129">Связи</span><span class="sxs-lookup"><span data-stu-id="ecad7-129">Relationships</span></span>
<span data-ttu-id="ecad7-130">Нет</span><span class="sxs-lookup"><span data-stu-id="ecad7-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ecad7-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ecad7-131">JSON Representation</span></span>
<span data-ttu-id="ecad7-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ecad7-132">Here is a JSON representation of the resource.</span></span>
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




