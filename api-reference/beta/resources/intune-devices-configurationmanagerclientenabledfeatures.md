---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9517bb807ad257ddba94b991223b781e91bbbc68
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890092"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="b00ef-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="b00ef-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="b00ef-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b00ef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b00ef-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b00ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b00ef-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b00ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b00ef-107">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="b00ef-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="b00ef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b00ef-108">Properties</span></span>
|<span data-ttu-id="b00ef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b00ef-109">Property</span></span>|<span data-ttu-id="b00ef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b00ef-110">Type</span></span>|<span data-ttu-id="b00ef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b00ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b00ef-112">inventory</span><span class="sxs-lookup"><span data-stu-id="b00ef-112">inventory</span></span>|<span data-ttu-id="b00ef-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="b00ef-113">Boolean</span></span>|<span data-ttu-id="b00ef-114">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="b00ef-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="b00ef-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="b00ef-115">modernApps</span></span>|<span data-ttu-id="b00ef-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="b00ef-116">Boolean</span></span>|<span data-ttu-id="b00ef-117">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="b00ef-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="b00ef-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="b00ef-118">resourceAccess</span></span>|<span data-ttu-id="b00ef-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="b00ef-119">Boolean</span></span>|<span data-ttu-id="b00ef-120">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="b00ef-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="b00ef-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b00ef-121">deviceConfiguration</span></span>|<span data-ttu-id="b00ef-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="b00ef-122">Boolean</span></span>|<span data-ttu-id="b00ef-123">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="b00ef-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="b00ef-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b00ef-124">compliancePolicy</span></span>|<span data-ttu-id="b00ef-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="b00ef-125">Boolean</span></span>|<span data-ttu-id="b00ef-126">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="b00ef-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="b00ef-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="b00ef-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="b00ef-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="b00ef-128">Boolean</span></span>|<span data-ttu-id="b00ef-129">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="b00ef-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="b00ef-130">Связи</span><span class="sxs-lookup"><span data-stu-id="b00ef-130">Relationships</span></span>
<span data-ttu-id="b00ef-131">Нет</span><span class="sxs-lookup"><span data-stu-id="b00ef-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b00ef-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b00ef-132">JSON Representation</span></span>
<span data-ttu-id="b00ef-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b00ef-133">Here is a JSON representation of the resource.</span></span>
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





