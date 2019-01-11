---
title: Тип ресурса managedDeviceCleanupSettings
description: Определение правила, когда администратор хочет устройств, чтобы очистить.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 755fc90b957427c4b9f8ee9007decea320141601
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808976"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="00f02-103">Тип ресурса managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="00f02-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="00f02-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="00f02-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00f02-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="00f02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="00f02-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00f02-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00f02-107">Определение правила, когда администратор хочет устройств, чтобы очистить.</span><span class="sxs-lookup"><span data-stu-id="00f02-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="00f02-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="00f02-108">Properties</span></span>
|<span data-ttu-id="00f02-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="00f02-109">Property</span></span>|<span data-ttu-id="00f02-110">Тип</span><span class="sxs-lookup"><span data-stu-id="00f02-110">Type</span></span>|<span data-ttu-id="00f02-111">Описание</span><span class="sxs-lookup"><span data-stu-id="00f02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00f02-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="00f02-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="00f02-113">Строка</span><span class="sxs-lookup"><span data-stu-id="00f02-113">String</span></span>|<span data-ttu-id="00f02-114">Количество дней, когда устройство имеет не связаться с Intune.</span><span class="sxs-lookup"><span data-stu-id="00f02-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="00f02-115">Связи</span><span class="sxs-lookup"><span data-stu-id="00f02-115">Relationships</span></span>
<span data-ttu-id="00f02-116">Нет</span><span class="sxs-lookup"><span data-stu-id="00f02-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="00f02-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00f02-117">JSON Representation</span></span>
<span data-ttu-id="00f02-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00f02-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceCleanupSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceCleanupSettings",
  "deviceInactivityBeforeRetirementInDays": "String"
}
```





