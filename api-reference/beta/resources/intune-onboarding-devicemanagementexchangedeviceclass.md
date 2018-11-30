---
title: Тип ресурса deviceManagementExchangeDeviceClass
description: Класс устройств в Exchange.
ms.openlocfilehash: 53234a97ffd2581eea1a4c480161ec9243a710d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27081564"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="6ae5a-103">Тип ресурса deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="6ae5a-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="6ae5a-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="6ae5a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ae5a-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ae5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ae5a-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6ae5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ae5a-107">Класс устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="6ae5a-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="6ae5a-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ae5a-108">Properties</span></span>
|<span data-ttu-id="6ae5a-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ae5a-109">Property</span></span>|<span data-ttu-id="6ae5a-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6ae5a-110">Type</span></span>|<span data-ttu-id="6ae5a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6ae5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ae5a-112">name</span><span class="sxs-lookup"><span data-stu-id="6ae5a-112">name</span></span>|<span data-ttu-id="6ae5a-113">String</span><span class="sxs-lookup"><span data-stu-id="6ae5a-113">String</span></span>|<span data-ttu-id="6ae5a-114">Имя класса устройства, которое будет затронут этого правила.</span><span class="sxs-lookup"><span data-stu-id="6ae5a-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="6ae5a-115">type</span><span class="sxs-lookup"><span data-stu-id="6ae5a-115">type</span></span>|[<span data-ttu-id="6ae5a-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="6ae5a-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="6ae5a-117">Тип устройства, который влияет этот правило семейства, например модели.</span><span class="sxs-lookup"><span data-stu-id="6ae5a-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="6ae5a-118">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="6ae5a-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ae5a-119">Связи</span><span class="sxs-lookup"><span data-stu-id="6ae5a-119">Relationships</span></span>
<span data-ttu-id="6ae5a-120">Нет</span><span class="sxs-lookup"><span data-stu-id="6ae5a-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ae5a-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ae5a-121">JSON Representation</span></span>
<span data-ttu-id="6ae5a-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ae5a-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeDeviceClass",
  "name": "String",
  "type": "String"
}
```





