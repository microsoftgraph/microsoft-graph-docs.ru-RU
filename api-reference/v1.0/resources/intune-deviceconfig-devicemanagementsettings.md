---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d36ab0a845450d803b3f0ac3fb0b9ea58cc4d3d3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460935"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="c733e-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c733e-103">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="c733e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c733e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c733e-105">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c733e-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c733e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c733e-106">Properties</span></span>
|<span data-ttu-id="c733e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c733e-107">Property</span></span>|<span data-ttu-id="c733e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c733e-108">Type</span></span>|<span data-ttu-id="c733e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c733e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c733e-110">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="c733e-110">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="c733e-111">Int32</span><span class="sxs-lookup"><span data-stu-id="c733e-111">Int32</span></span>|<span data-ttu-id="c733e-112">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="c733e-112">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="c733e-113">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="c733e-113">Valid values 0 to 120</span></span>|
|<span data-ttu-id="c733e-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="c733e-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="c733e-115">Логический</span><span class="sxs-lookup"><span data-stu-id="c733e-115">Boolean</span></span>|<span data-ttu-id="c733e-116">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="c733e-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="c733e-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="c733e-117">secureByDefault</span></span>|<span data-ttu-id="c733e-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c733e-118">Boolean</span></span>|<span data-ttu-id="c733e-119">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c733e-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="c733e-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="c733e-120">Relationships</span></span>
<span data-ttu-id="c733e-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c733e-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c733e-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c733e-122">JSON Representation</span></span>
<span data-ttu-id="c733e-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c733e-123">Here is a JSON representation of the resource.</span></span>
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



