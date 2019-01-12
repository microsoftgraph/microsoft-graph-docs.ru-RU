---
title: Тип ресурса deviceManagementExchangeAccessRule
description: Правила доступа устройств в Exchange.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a03fb9f56361cc72bd0321a3b2bd548571740b34
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27927816"
---
# <a name="devicemanagementexchangeaccessrule-resource-type"></a><span data-ttu-id="e300a-103">Тип ресурса deviceManagementExchangeAccessRule</span><span class="sxs-lookup"><span data-stu-id="e300a-103">deviceManagementExchangeAccessRule resource type</span></span>

> <span data-ttu-id="e300a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e300a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e300a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e300a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e300a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e300a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e300a-107">Правила доступа устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e300a-107">Device Access Rules in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="e300a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e300a-108">Properties</span></span>
|<span data-ttu-id="e300a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e300a-109">Property</span></span>|<span data-ttu-id="e300a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e300a-110">Type</span></span>|<span data-ttu-id="e300a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e300a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e300a-112">deviceClass</span><span class="sxs-lookup"><span data-stu-id="e300a-112">deviceClass</span></span>|[<span data-ttu-id="e300a-113">deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="e300a-113">deviceManagementExchangeDeviceClass</span></span>](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)|<span data-ttu-id="e300a-114">Класс устройства, который будет затронут этого правила.</span><span class="sxs-lookup"><span data-stu-id="e300a-114">Device Class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="e300a-115">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e300a-115">accessLevel</span></span>|[<span data-ttu-id="e300a-116">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="e300a-116">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="e300a-117">Уровень доступа для Exchange, предоставленных с этого правила.</span><span class="sxs-lookup"><span data-stu-id="e300a-117">Access Level for Exchange granted by this rule.</span></span> <span data-ttu-id="e300a-118">Возможные значения: `none`, `allow`, `block`, `quarantine`.</span><span class="sxs-lookup"><span data-stu-id="e300a-118">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e300a-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e300a-119">Relationships</span></span>
<span data-ttu-id="e300a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e300a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e300a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e300a-121">JSON Representation</span></span>
<span data-ttu-id="e300a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e300a-122">Here is a JSON representation of the resource.</span></span>
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





