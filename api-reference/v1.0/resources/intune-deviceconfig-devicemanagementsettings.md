---
title: Тип ресурса deviceManagementSettings
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3742262f2d17cdac1344379b39b4891b5b9919ec
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830592"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="981f3-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="981f3-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="981f3-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="981f3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="981f3-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="981f3-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="981f3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="981f3-106">Properties</span></span>
|<span data-ttu-id="981f3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="981f3-107">Property</span></span>|<span data-ttu-id="981f3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="981f3-108">Type</span></span>|<span data-ttu-id="981f3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="981f3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="981f3-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="981f3-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="981f3-111">Int32</span><span class="sxs-lookup"><span data-stu-id="981f3-111">Int32</span></span>|<span data-ttu-id="981f3-112">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="981f3-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="981f3-113">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="981f3-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="981f3-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="981f3-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="981f3-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="981f3-115">Boolean</span></span>|<span data-ttu-id="981f3-116">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="981f3-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="981f3-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="981f3-117">secureByDefault</span></span>|<span data-ttu-id="981f3-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="981f3-118">Boolean</span></span>|<span data-ttu-id="981f3-119">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="981f3-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="981f3-120">Связи</span><span class="sxs-lookup"><span data-stu-id="981f3-120">Relationships</span></span>
<span data-ttu-id="981f3-121">Нет</span><span class="sxs-lookup"><span data-stu-id="981f3-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="981f3-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="981f3-122">JSON Representation</span></span>
<span data-ttu-id="981f3-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="981f3-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



