---
title: Тип ресурса deviceManagementSettings
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f973f2645b37375641bc536b5ace0fa508fb0b0e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854420"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="0855c-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="0855c-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="0855c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="0855c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0855c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0855c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0855c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0855c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0855c-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="0855c-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="0855c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0855c-108">Properties</span></span>
|<span data-ttu-id="0855c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0855c-109">Property</span></span>|<span data-ttu-id="0855c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0855c-110">Type</span></span>|<span data-ttu-id="0855c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0855c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0855c-112">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="0855c-112">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="0855c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0855c-113">Int32</span></span>|<span data-ttu-id="0855c-114">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="0855c-114">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="0855c-115">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="0855c-115">Valid values 0 to 120</span></span>|
|<span data-ttu-id="0855c-116">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="0855c-116">isScheduledActionEnabled</span></span>|<span data-ttu-id="0855c-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="0855c-117">Boolean</span></span>|<span data-ttu-id="0855c-118">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="0855c-118">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="0855c-119">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="0855c-119">secureByDefault</span></span>|<span data-ttu-id="0855c-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="0855c-120">Boolean</span></span>|<span data-ttu-id="0855c-121">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="0855c-121">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|
|<span data-ttu-id="0855c-122">enhancedJailBreak</span><span class="sxs-lookup"><span data-stu-id="0855c-122">enhancedJailBreak</span></span>|<span data-ttu-id="0855c-123">Логический</span><span class="sxs-lookup"><span data-stu-id="0855c-123">Boolean</span></span>|<span data-ttu-id="0855c-124">— Это функция включена или не для улучшения обнаружения jailbreak.</span><span class="sxs-lookup"><span data-stu-id="0855c-124">Is feature enabled or not for enhanced jailbreak detection.</span></span>|
|<span data-ttu-id="0855c-125">deviceInactivityBeforeRetirementInDay</span><span class="sxs-lookup"><span data-stu-id="0855c-125">deviceInactivityBeforeRetirementInDay</span></span>|<span data-ttu-id="0855c-126">Int32</span><span class="sxs-lookup"><span data-stu-id="0855c-126">Int32</span></span>|<span data-ttu-id="0855c-127">Когда устройство не проверяет, для указанного числа дней, компании данных может быть удален, устройство не будет в разделе Управление.</span><span class="sxs-lookup"><span data-stu-id="0855c-127">When the device does not check in for specified number of days, the company data might be removed and the device will not be under management.</span></span> <span data-ttu-id="0855c-128">Допустимые значения 30 на 270 градусов</span><span class="sxs-lookup"><span data-stu-id="0855c-128">Valid values 30 to 270</span></span>|

## <a name="relationships"></a><span data-ttu-id="0855c-129">Связи</span><span class="sxs-lookup"><span data-stu-id="0855c-129">Relationships</span></span>
<span data-ttu-id="0855c-130">Нет</span><span class="sxs-lookup"><span data-stu-id="0855c-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0855c-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0855c-131">JSON Representation</span></span>
<span data-ttu-id="0855c-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0855c-132">Here is a JSON representation of the resource.</span></span>
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
  "secureByDefault": true,
  "enhancedJailBreak": true,
  "deviceInactivityBeforeRetirementInDay": 1024
}
```





