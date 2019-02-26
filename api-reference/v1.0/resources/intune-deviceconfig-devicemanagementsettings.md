---
title: Тип ресурса deviceManagementSettings
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d36ab0a845450d803b3f0ac3fb0b9ea58cc4d3d3
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250798"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="71cbc-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="71cbc-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="71cbc-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="71cbc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71cbc-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="71cbc-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="71cbc-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="71cbc-106">Properties</span></span>
|<span data-ttu-id="71cbc-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="71cbc-107">Property</span></span>|<span data-ttu-id="71cbc-108">Тип</span><span class="sxs-lookup"><span data-stu-id="71cbc-108">Type</span></span>|<span data-ttu-id="71cbc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="71cbc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71cbc-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="71cbc-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="71cbc-111">Int32</span><span class="sxs-lookup"><span data-stu-id="71cbc-111">Int32</span></span>|<span data-ttu-id="71cbc-112">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="71cbc-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="71cbc-113">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="71cbc-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="71cbc-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="71cbc-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="71cbc-115">Логический</span><span class="sxs-lookup"><span data-stu-id="71cbc-115">Boolean</span></span>|<span data-ttu-id="71cbc-116">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="71cbc-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="71cbc-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="71cbc-117">secureByDefault</span></span>|<span data-ttu-id="71cbc-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="71cbc-118">Boolean</span></span>|<span data-ttu-id="71cbc-119">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="71cbc-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="71cbc-120">Связи</span><span class="sxs-lookup"><span data-stu-id="71cbc-120">Relationships</span></span>
<span data-ttu-id="71cbc-121">Нет</span><span class="sxs-lookup"><span data-stu-id="71cbc-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71cbc-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="71cbc-122">JSON Representation</span></span>
<span data-ttu-id="71cbc-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71cbc-123">Here is a JSON representation of the resource.</span></span>
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



