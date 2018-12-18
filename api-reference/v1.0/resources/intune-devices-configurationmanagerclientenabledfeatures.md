---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
author: tfitzmac
ms.openlocfilehash: fe975f2e8d537d1231a89eb9f2a44cdd8258fd1a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27325146"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="b8b91-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="b8b91-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="b8b91-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b8b91-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8b91-105">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="b8b91-105">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="b8b91-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b8b91-106">Properties</span></span>
|<span data-ttu-id="b8b91-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b8b91-107">Property</span></span>|<span data-ttu-id="b8b91-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b8b91-108">Type</span></span>|<span data-ttu-id="b8b91-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b8b91-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8b91-110">inventory</span><span class="sxs-lookup"><span data-stu-id="b8b91-110">inventory</span></span>|<span data-ttu-id="b8b91-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8b91-111">Boolean</span></span>|<span data-ttu-id="b8b91-112">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="b8b91-112">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="b8b91-113">modernApps</span><span class="sxs-lookup"><span data-stu-id="b8b91-113">modernApps</span></span>|<span data-ttu-id="b8b91-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8b91-114">Boolean</span></span>|<span data-ttu-id="b8b91-115">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="b8b91-115">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="b8b91-116">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="b8b91-116">resourceAccess</span></span>|<span data-ttu-id="b8b91-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8b91-117">Boolean</span></span>|<span data-ttu-id="b8b91-118">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="b8b91-118">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="b8b91-119">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b8b91-119">deviceConfiguration</span></span>|<span data-ttu-id="b8b91-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8b91-120">Boolean</span></span>|<span data-ttu-id="b8b91-121">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="b8b91-121">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="b8b91-122">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="b8b91-122">compliancePolicy</span></span>|<span data-ttu-id="b8b91-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8b91-123">Boolean</span></span>|<span data-ttu-id="b8b91-124">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="b8b91-124">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="b8b91-125">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="b8b91-125">windowsUpdateForBusiness</span></span>|<span data-ttu-id="b8b91-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="b8b91-126">Boolean</span></span>|<span data-ttu-id="b8b91-127">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="b8b91-127">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8b91-128">Связи</span><span class="sxs-lookup"><span data-stu-id="b8b91-128">Relationships</span></span>
<span data-ttu-id="b8b91-129">Нет</span><span class="sxs-lookup"><span data-stu-id="b8b91-129">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8b91-130">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b8b91-130">JSON Representation</span></span>
<span data-ttu-id="b8b91-131">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b8b91-131">Here is a JSON representation of the resource.</span></span>
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



