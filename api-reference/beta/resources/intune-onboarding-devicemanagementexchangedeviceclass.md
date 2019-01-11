---
title: Тип ресурса deviceManagementExchangeDeviceClass
description: Класс устройств в Exchange.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 80142f4e05752a37c324cd20ce96e4c8e6668c03
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839027"
---
# <a name="devicemanagementexchangedeviceclass-resource-type"></a><span data-ttu-id="88d75-103">Тип ресурса deviceManagementExchangeDeviceClass</span><span class="sxs-lookup"><span data-stu-id="88d75-103">deviceManagementExchangeDeviceClass resource type</span></span>

> <span data-ttu-id="88d75-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="88d75-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88d75-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="88d75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88d75-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="88d75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88d75-107">Класс устройств в Exchange.</span><span class="sxs-lookup"><span data-stu-id="88d75-107">Device Class in Exchange.</span></span>
## <a name="properties"></a><span data-ttu-id="88d75-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="88d75-108">Properties</span></span>
|<span data-ttu-id="88d75-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="88d75-109">Property</span></span>|<span data-ttu-id="88d75-110">Тип</span><span class="sxs-lookup"><span data-stu-id="88d75-110">Type</span></span>|<span data-ttu-id="88d75-111">Описание</span><span class="sxs-lookup"><span data-stu-id="88d75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88d75-112">name</span><span class="sxs-lookup"><span data-stu-id="88d75-112">name</span></span>|<span data-ttu-id="88d75-113">Строка</span><span class="sxs-lookup"><span data-stu-id="88d75-113">String</span></span>|<span data-ttu-id="88d75-114">Имя класса устройства, которое будет затронут этого правила.</span><span class="sxs-lookup"><span data-stu-id="88d75-114">Name of the device class which will be impacted by this rule.</span></span>|
|<span data-ttu-id="88d75-115">type</span><span class="sxs-lookup"><span data-stu-id="88d75-115">type</span></span>|[<span data-ttu-id="88d75-116">deviceManagementExchangeAccessRuleType</span><span class="sxs-lookup"><span data-stu-id="88d75-116">deviceManagementExchangeAccessRuleType</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccessruletype.md)|<span data-ttu-id="88d75-117">Тип устройства, который влияет этот правило семейства, например модели.</span><span class="sxs-lookup"><span data-stu-id="88d75-117">Type of device which is impacted by this rule e.g. Model, Family.</span></span> <span data-ttu-id="88d75-118">Возможные значения: `family`, `model`.</span><span class="sxs-lookup"><span data-stu-id="88d75-118">Possible values are: `family`, `model`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="88d75-119">Связи</span><span class="sxs-lookup"><span data-stu-id="88d75-119">Relationships</span></span>
<span data-ttu-id="88d75-120">Нет</span><span class="sxs-lookup"><span data-stu-id="88d75-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="88d75-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="88d75-121">JSON Representation</span></span>
<span data-ttu-id="88d75-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="88d75-122">Here is a JSON representation of the resource.</span></span>
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





