---
title: Тип ресурса Андроидманажедстореапптракк
description: Содержит сведения о записях для приложений управляемого хранилища Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0444165a3dfb86efa1f4fc25e2edf0ea309b6959
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004076"
---
# <a name="androidmanagedstoreapptrack-resource-type"></a><span data-ttu-id="8589e-103">Тип ресурса Андроидманажедстореапптракк</span><span class="sxs-lookup"><span data-stu-id="8589e-103">androidManagedStoreAppTrack resource type</span></span>

<span data-ttu-id="8589e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8589e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8589e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8589e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8589e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8589e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8589e-107">Содержит сведения о записях для приложений управляемого хранилища Android.</span><span class="sxs-lookup"><span data-stu-id="8589e-107">Contains track information for Android Managed Store apps.</span></span>

## <a name="properties"></a><span data-ttu-id="8589e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="8589e-108">Properties</span></span>
|<span data-ttu-id="8589e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="8589e-109">Property</span></span>|<span data-ttu-id="8589e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="8589e-110">Type</span></span>|<span data-ttu-id="8589e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8589e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8589e-112">траккид</span><span class="sxs-lookup"><span data-stu-id="8589e-112">trackId</span></span>|<span data-ttu-id="8589e-113">String</span><span class="sxs-lookup"><span data-stu-id="8589e-113">String</span></span>|<span data-ttu-id="8589e-114">Уникальный идентификатор записи.</span><span class="sxs-lookup"><span data-stu-id="8589e-114">Unique track identifier.</span></span>|
|<span data-ttu-id="8589e-115">траккалиас</span><span class="sxs-lookup"><span data-stu-id="8589e-115">trackAlias</span></span>|<span data-ttu-id="8589e-116">String</span><span class="sxs-lookup"><span data-stu-id="8589e-116">String</span></span>|<span data-ttu-id="8589e-117">Понятное имя для отслеживания.</span><span class="sxs-lookup"><span data-stu-id="8589e-117">Friendly name for track.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8589e-118">Связи</span><span class="sxs-lookup"><span data-stu-id="8589e-118">Relationships</span></span>
<span data-ttu-id="8589e-119">Нет</span><span class="sxs-lookup"><span data-stu-id="8589e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8589e-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8589e-120">JSON Representation</span></span>
<span data-ttu-id="8589e-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8589e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidManagedStoreAppTrack"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidManagedStoreAppTrack",
  "trackId": "String",
  "trackAlias": "String"
}
```






