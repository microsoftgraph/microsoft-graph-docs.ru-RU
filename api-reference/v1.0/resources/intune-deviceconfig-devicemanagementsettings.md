---
title: Тип ресурса deviceManagementSettings
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 9e444f0a92a2e28dfa571c51f08c886537701f3a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343612"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="08b59-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="08b59-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="08b59-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="08b59-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="08b59-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="08b59-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="08b59-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="08b59-106">Properties</span></span>
|<span data-ttu-id="08b59-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="08b59-107">Property</span></span>|<span data-ttu-id="08b59-108">Тип</span><span class="sxs-lookup"><span data-stu-id="08b59-108">Type</span></span>|<span data-ttu-id="08b59-109">Описание</span><span class="sxs-lookup"><span data-stu-id="08b59-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08b59-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="08b59-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="08b59-111">Int32</span><span class="sxs-lookup"><span data-stu-id="08b59-111">Int32</span></span>|<span data-ttu-id="08b59-112">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="08b59-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="08b59-113">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="08b59-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="08b59-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="08b59-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="08b59-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="08b59-115">Boolean</span></span>|<span data-ttu-id="08b59-116">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="08b59-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="08b59-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="08b59-117">secureByDefault</span></span>|<span data-ttu-id="08b59-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="08b59-118">Boolean</span></span>|<span data-ttu-id="08b59-119">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="08b59-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="08b59-120">Связи</span><span class="sxs-lookup"><span data-stu-id="08b59-120">Relationships</span></span>
<span data-ttu-id="08b59-121">Нет</span><span class="sxs-lookup"><span data-stu-id="08b59-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="08b59-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08b59-122">JSON Representation</span></span>
<span data-ttu-id="08b59-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08b59-123">Here is a JSON representation of the resource.</span></span>
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



