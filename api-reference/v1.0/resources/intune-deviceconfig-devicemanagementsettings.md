---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 17856c01f006206298e1efa1ed01fdcac6045557
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755100"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="c0b52-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="c0b52-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="c0b52-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0b52-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0b52-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0b52-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0b52-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c0b52-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c0b52-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0b52-107">Properties</span></span>
|<span data-ttu-id="c0b52-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0b52-108">Property</span></span>|<span data-ttu-id="c0b52-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c0b52-109">Type</span></span>|<span data-ttu-id="c0b52-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c0b52-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0b52-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="c0b52-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="c0b52-112">Int32</span><span class="sxs-lookup"><span data-stu-id="c0b52-112">Int32</span></span>|<span data-ttu-id="c0b52-113">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="c0b52-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span>|
|<span data-ttu-id="c0b52-114">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="c0b52-114">isScheduledActionEnabled</span></span>|<span data-ttu-id="c0b52-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b52-115">Boolean</span></span>|<span data-ttu-id="c0b52-116">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="c0b52-116">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="c0b52-117">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="c0b52-117">secureByDefault</span></span>|<span data-ttu-id="c0b52-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="c0b52-118">Boolean</span></span>|<span data-ttu-id="c0b52-119">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="c0b52-119">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0b52-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="c0b52-120">Relationships</span></span>
<span data-ttu-id="c0b52-121">Нет</span><span class="sxs-lookup"><span data-stu-id="c0b52-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0b52-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0b52-122">JSON Representation</span></span>
<span data-ttu-id="c0b52-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0b52-123">Here is a JSON representation of the resource.</span></span>
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




