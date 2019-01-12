---
title: Тип ресурса managedDeviceCleanupSettings
description: Определение правила, когда администратор хочет устройств, чтобы очистить.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 334b561ffa19d4161553f761ce65b7da7d9dbcfa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961899"
---
# <a name="manageddevicecleanupsettings-resource-type"></a><span data-ttu-id="23a13-103">Тип ресурса managedDeviceCleanupSettings</span><span class="sxs-lookup"><span data-stu-id="23a13-103">managedDeviceCleanupSettings resource type</span></span>

> <span data-ttu-id="23a13-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="23a13-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23a13-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23a13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23a13-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="23a13-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23a13-107">Определение правила, когда администратор хочет устройств, чтобы очистить.</span><span class="sxs-lookup"><span data-stu-id="23a13-107">Define the rule when the admin wants the devices to be cleaned up.</span></span>
## <a name="properties"></a><span data-ttu-id="23a13-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="23a13-108">Properties</span></span>
|<span data-ttu-id="23a13-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="23a13-109">Property</span></span>|<span data-ttu-id="23a13-110">Тип</span><span class="sxs-lookup"><span data-stu-id="23a13-110">Type</span></span>|<span data-ttu-id="23a13-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23a13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23a13-112">deviceInactivityBeforeRetirementInDays</span><span class="sxs-lookup"><span data-stu-id="23a13-112">deviceInactivityBeforeRetirementInDays</span></span>|<span data-ttu-id="23a13-113">Строка</span><span class="sxs-lookup"><span data-stu-id="23a13-113">String</span></span>|<span data-ttu-id="23a13-114">Количество дней, когда устройство имеет не связаться с Intune.</span><span class="sxs-lookup"><span data-stu-id="23a13-114">Number of days when the device has not contacted Intune.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23a13-115">Связи</span><span class="sxs-lookup"><span data-stu-id="23a13-115">Relationships</span></span>
<span data-ttu-id="23a13-116">Нет</span><span class="sxs-lookup"><span data-stu-id="23a13-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23a13-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23a13-117">JSON Representation</span></span>
<span data-ttu-id="23a13-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23a13-118">Here is a JSON representation of the resource.</span></span>
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





