---
title: Тип ресурса configurationManagerClientEnabledFeatures
description: Включенные клиентом функции диспетчера конфигураций
ms.openlocfilehash: 60d0e9e78bc4b641bb1f9ee0d61cc09744500424
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076173"
---
# <a name="configurationmanagerclientenabledfeatures-resource-type"></a><span data-ttu-id="c8dcf-103">Тип ресурса configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="c8dcf-103">configurationManagerClientEnabledFeatures resource type</span></span>

> <span data-ttu-id="c8dcf-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8dcf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8dcf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8dcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8dcf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8dcf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8dcf-107">Включенные клиентом функции диспетчера конфигураций</span><span class="sxs-lookup"><span data-stu-id="c8dcf-107">configuration Manager client enabled features</span></span>
## <a name="properties"></a><span data-ttu-id="c8dcf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8dcf-108">Properties</span></span>
|<span data-ttu-id="c8dcf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8dcf-109">Property</span></span>|<span data-ttu-id="c8dcf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c8dcf-110">Type</span></span>|<span data-ttu-id="c8dcf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c8dcf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8dcf-112">inventory</span><span class="sxs-lookup"><span data-stu-id="c8dcf-112">inventory</span></span>|<span data-ttu-id="c8dcf-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8dcf-113">Boolean</span></span>|<span data-ttu-id="c8dcf-114">Управляет ли Intune данными инвентаризации</span><span class="sxs-lookup"><span data-stu-id="c8dcf-114">Whether inventory is managed by Intune</span></span>|
|<span data-ttu-id="c8dcf-115">modernApps</span><span class="sxs-lookup"><span data-stu-id="c8dcf-115">modernApps</span></span>|<span data-ttu-id="c8dcf-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8dcf-116">Boolean</span></span>|<span data-ttu-id="c8dcf-117">Управляет ли Intune современным приложением</span><span class="sxs-lookup"><span data-stu-id="c8dcf-117">Whether modern application is managed by Intune</span></span>|
|<span data-ttu-id="c8dcf-118">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="c8dcf-118">resourceAccess</span></span>|<span data-ttu-id="c8dcf-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8dcf-119">Boolean</span></span>|<span data-ttu-id="c8dcf-120">Управляет ли Intune доступом к ресурсам</span><span class="sxs-lookup"><span data-stu-id="c8dcf-120">Whether resource access is managed by Intune</span></span>|
|<span data-ttu-id="c8dcf-121">deviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c8dcf-121">deviceConfiguration</span></span>|<span data-ttu-id="c8dcf-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8dcf-122">Boolean</span></span>|<span data-ttu-id="c8dcf-123">Управляет ли Intune конфигурацией устройства</span><span class="sxs-lookup"><span data-stu-id="c8dcf-123">Whether device configuration is managed by Intune</span></span>|
|<span data-ttu-id="c8dcf-124">compliancePolicy</span><span class="sxs-lookup"><span data-stu-id="c8dcf-124">compliancePolicy</span></span>|<span data-ttu-id="c8dcf-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8dcf-125">Boolean</span></span>|<span data-ttu-id="c8dcf-126">Управляется ли Intune политикой соответствия требованиям</span><span class="sxs-lookup"><span data-stu-id="c8dcf-126">Whether compliance policy is managed by Intune</span></span>|
|<span data-ttu-id="c8dcf-127">windowsUpdateForBusiness</span><span class="sxs-lookup"><span data-stu-id="c8dcf-127">windowsUpdateForBusiness</span></span>|<span data-ttu-id="c8dcf-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="c8dcf-128">Boolean</span></span>|<span data-ttu-id="c8dcf-129">Управляет ли Intune Центром обновления Windows для бизнеса</span><span class="sxs-lookup"><span data-stu-id="c8dcf-129">Whether Windows Update for Business is managed by Intune</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8dcf-130">Связи</span><span class="sxs-lookup"><span data-stu-id="c8dcf-130">Relationships</span></span>
<span data-ttu-id="c8dcf-131">Нет</span><span class="sxs-lookup"><span data-stu-id="c8dcf-131">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8dcf-132">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8dcf-132">JSON Representation</span></span>
<span data-ttu-id="c8dcf-133">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8dcf-133">Here is a JSON representation of the resource.</span></span>
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





