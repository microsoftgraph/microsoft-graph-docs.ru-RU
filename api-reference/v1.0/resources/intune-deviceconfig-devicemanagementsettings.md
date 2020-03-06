---
title: Тип ресурса deviceManagementSettings
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 24ee75e414411f046577bf31893c82541980b277
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532563"
---
# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="41f81-103">Тип ресурса deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="41f81-103">deviceManagementSettings resource type</span></span>

<span data-ttu-id="41f81-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41f81-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="41f81-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="41f81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41f81-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="41f81-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="41f81-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="41f81-107">Properties</span></span>
|<span data-ttu-id="41f81-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="41f81-108">Property</span></span>|<span data-ttu-id="41f81-109">Тип</span><span class="sxs-lookup"><span data-stu-id="41f81-109">Type</span></span>|<span data-ttu-id="41f81-110">Описание</span><span class="sxs-lookup"><span data-stu-id="41f81-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41f81-111">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="41f81-111">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="41f81-112">Int32</span><span class="sxs-lookup"><span data-stu-id="41f81-112">Int32</span></span>|<span data-ttu-id="41f81-113">Количество дней, в течение которых устройство может считаться соответствующим требованиям, несмотря на отсутствие записей после изменения.</span><span class="sxs-lookup"><span data-stu-id="41f81-113">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="41f81-114">Допустимые значения: от 0 до 120</span><span class="sxs-lookup"><span data-stu-id="41f81-114">Valid values 0 to 120</span></span>|
|<span data-ttu-id="41f81-115">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="41f81-115">isScheduledActionEnabled</span></span>|<span data-ttu-id="41f81-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f81-116">Boolean</span></span>|<span data-ttu-id="41f81-117">Включена ли функция для запланированного действия для правила.</span><span class="sxs-lookup"><span data-stu-id="41f81-117">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="41f81-118">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="41f81-118">secureByDefault</span></span>|<span data-ttu-id="41f81-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="41f81-119">Boolean</span></span>|<span data-ttu-id="41f81-120">Устройство считается несоответствующим требованиям, если для данного свойства установлено значение true, но не выбраны целевые политики соответствия требованиям.</span><span class="sxs-lookup"><span data-stu-id="41f81-120">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="41f81-121">Связи</span><span class="sxs-lookup"><span data-stu-id="41f81-121">Relationships</span></span>
<span data-ttu-id="41f81-122">Нет</span><span class="sxs-lookup"><span data-stu-id="41f81-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41f81-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="41f81-123">JSON Representation</span></span>
<span data-ttu-id="41f81-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="41f81-124">Here is a JSON representation of the resource.</span></span>
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




