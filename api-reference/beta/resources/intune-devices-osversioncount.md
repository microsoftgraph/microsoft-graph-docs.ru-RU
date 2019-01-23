---
title: Тип ресурса osVersionCount
description: Количество устройств с вредоносных программ для каждой версии операционной системы
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cbe0d8ac149ad84ba4cd1286fb0f2303cdfb52a1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410464"
---
# <a name="osversioncount-resource-type"></a><span data-ttu-id="ca520-103">Тип ресурса osVersionCount</span><span class="sxs-lookup"><span data-stu-id="ca520-103">osVersionCount resource type</span></span>

> <span data-ttu-id="ca520-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ca520-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ca520-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ca520-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca520-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca520-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca520-107">Количество устройств с вредоносных программ для каждой версии операционной системы</span><span class="sxs-lookup"><span data-stu-id="ca520-107">Count of devices with malware for each OS version</span></span>

## <a name="properties"></a><span data-ttu-id="ca520-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca520-108">Properties</span></span>
|<span data-ttu-id="ca520-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca520-109">Property</span></span>|<span data-ttu-id="ca520-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ca520-110">Type</span></span>|<span data-ttu-id="ca520-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ca520-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca520-112">osVersion</span><span class="sxs-lookup"><span data-stu-id="ca520-112">osVersion</span></span>|<span data-ttu-id="ca520-113">String</span><span class="sxs-lookup"><span data-stu-id="ca520-113">String</span></span>|<span data-ttu-id="ca520-114">Версия операционной системы</span><span class="sxs-lookup"><span data-stu-id="ca520-114">OS version</span></span>|
|<span data-ttu-id="ca520-115">deviceCount</span><span class="sxs-lookup"><span data-stu-id="ca520-115">deviceCount</span></span>|<span data-ttu-id="ca520-116">Int32</span><span class="sxs-lookup"><span data-stu-id="ca520-116">Int32</span></span>|<span data-ttu-id="ca520-117">Количество устройств с вредоносных программ для версии операционной системы</span><span class="sxs-lookup"><span data-stu-id="ca520-117">Count of devices with malware for the OS version</span></span>|
|<span data-ttu-id="ca520-118">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="ca520-118">lastUpdateDateTime</span></span>|<span data-ttu-id="ca520-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca520-119">DateTimeOffset</span></span>|<span data-ttu-id="ca520-120">Метка времени последнего обновления для счетчик устройства в формате UTC</span><span class="sxs-lookup"><span data-stu-id="ca520-120">The Timestamp of the last update for the device count in UTC</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca520-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="ca520-121">Relationships</span></span>
<span data-ttu-id="ca520-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ca520-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca520-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca520-123">JSON Representation</span></span>
<span data-ttu-id="ca520-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca520-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.osVersionCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.osVersionCount",
  "osVersion": "String",
  "deviceCount": 1024,
  "lastUpdateDateTime": "String (timestamp)"
}
```




