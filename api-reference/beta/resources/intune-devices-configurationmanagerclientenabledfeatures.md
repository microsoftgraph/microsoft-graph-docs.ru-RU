---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 07b143a8d61335c44c83d1d88b9a67d2d3c2e4dc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962088"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="0f5fb-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="0f5fb-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="0f5fb-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0f5fb-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0f5fb-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0f5fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0f5fb-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0f5fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0f5fb-107">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="0f5fb-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="0f5fb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0f5fb-108">Properties</span></span>
|<span data-ttu-id="0f5fb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0f5fb-109">Property</span></span>|<span data-ttu-id="0f5fb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0f5fb-110">Type</span></span>|<span data-ttu-id="0f5fb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0f5fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f5fb-112">inventory</span><span class="sxs-lookup"><span data-stu-id="0f5fb-112">inventory</span></span>|<span data-ttu-id="0f5fb-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5fb-113">Boolean</span></span>|<span data-ttu-id="0f5fb-114">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="0f5fb-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="0f5fb-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="0f5fb-115">modernApps</span></span>|<span data-ttu-id="0f5fb-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5fb-116">Boolean</span></span>|<span data-ttu-id="0f5fb-117">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="0f5fb-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="0f5fb-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="0f5fb-118">resourceAccess</span></span>|<span data-ttu-id="0f5fb-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5fb-119">Boolean</span></span>|<span data-ttu-id="0f5fb-120">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="0f5fb-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="0f5fb-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0f5fb-121">deviceConfiguration</span></span>|<span data-ttu-id="0f5fb-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5fb-122">Boolean</span></span>|<span data-ttu-id="0f5fb-123">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="0f5fb-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="0f5fb-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="0f5fb-124">compliancePolicy</span></span>|<span data-ttu-id="0f5fb-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5fb-125">Boolean</span></span>|<span data-ttu-id="0f5fb-126">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="0f5fb-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="0f5fb-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="0f5fb-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="0f5fb-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="0f5fb-128">Boolean</span></span>|<span data-ttu-id="0f5fb-129">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="0f5fb-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f5fb-130">Связи</span><span class="sxs-lookup"><span data-stu-id="0f5fb-130">Relationships</span></span>
<span data-ttu-id="0f5fb-131">Нет</span><span class="sxs-lookup"><span data-stu-id="0f5fb-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0f5fb-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0f5fb-132">JSON Representation</span></span>
<span data-ttu-id="0f5fb-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0f5fb-133">Here is a JSON representation of the resource.</span></span>
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





