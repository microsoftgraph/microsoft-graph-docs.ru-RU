---
title: Тип ресурса deviceManagementExchangeAccessRule
description: Правила доступа устройств в Exchange.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c46bff30bf5f88723a789bb13160bf5aedb1ef2a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409442"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="2fe41-103">Тип ресурса deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="2fe41-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="2fe41-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2fe41-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2fe41-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2fe41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fe41-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2fe41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fe41-107">Правила доступа устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2fe41-107">Device Access Rules in Exchange.</span></span>

## <a name="properties"></a><span data-ttu-id="2fe41-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2fe41-108">Properties</span></span>
|<span data-ttu-id="2fe41-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2fe41-109">Property</span></span>|<span data-ttu-id="2fe41-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2fe41-110">Type</span></span>|<span data-ttu-id="2fe41-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2fe41-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fe41-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="2fe41-112">deviceClass</span></span>|[<span data-ttu-id="2fe41-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="2fe41-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="2fe41-114">Класс устройства, который будет затронут этого правила.</span><span class="sxs-lookup"><span data-stu-id="2fe41-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="2fe41-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="2fe41-115">accessLevel</span></span>|[<span data-ttu-id="2fe41-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="2fe41-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="2fe41-117">Уровень доступа для Exchange, предоставленных с этого правила.</span><span class="sxs-lookup"><span data-stu-id="2fe41-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="2fe41-118">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="2fe41-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2fe41-119">Связи</span><span class="sxs-lookup"><span data-stu-id="2fe41-119">Relationships</span></span>
<span data-ttu-id="2fe41-120">Нет</span><span class="sxs-lookup"><span data-stu-id="2fe41-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2fe41-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2fe41-121">JSON Representation</span></span>
<span data-ttu-id="2fe41-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2fe41-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeAccessRule",
  "deviceClass": {
    "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
    "name": "String",
    "type": "String"
  },
  "accessLevel": "String"
}
```




