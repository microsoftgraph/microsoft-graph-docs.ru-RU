---
title: Тип ресурса managedDeviceCleanupSettings
description: Определение правила, когда администратор хочет устройств, чтобы очистить.
ms.openlocfilehash: f7782ac9d6571b58c8ed1e7964637736fcb5f3d4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078839"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="54920-103">Тип ресурса managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="54920-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="54920-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="54920-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54920-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="54920-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54920-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="54920-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="54920-107">Определение правила, когда администратор хочет устройств, чтобы очистить.</span><span class="sxs-lookup"><span data-stu-id="54920-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="54920-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="54920-108">Properties</span></span>
|<span data-ttu-id="54920-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="54920-109">Property</span></span>|<span data-ttu-id="54920-110">Тип</span><span class="sxs-lookup"><span data-stu-id="54920-110">Type</span></span>|<span data-ttu-id="54920-111">Description</span><span class="sxs-lookup"><span data-stu-id="54920-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54920-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="54920-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="54920-113">String</span><span class="sxs-lookup"><span data-stu-id="54920-113">String</span></span>|<span data-ttu-id="54920-114">Количество дней, когда устройство имеет не связаться с Intune.</span><span class="sxs-lookup"><span data-stu-id="54920-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="54920-115">Связи</span><span class="sxs-lookup"><span data-stu-id="54920-115">Relationships</span></span>
<span data-ttu-id="54920-116">Нет</span><span class="sxs-lookup"><span data-stu-id="54920-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="54920-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="54920-117">JSON Representation</span></span>
<span data-ttu-id="54920-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="54920-118">Here is a JSON representation of the resource.</span></span>
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





