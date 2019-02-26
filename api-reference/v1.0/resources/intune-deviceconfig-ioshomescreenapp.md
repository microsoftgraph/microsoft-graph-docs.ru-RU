---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67c11096414db0dccad2ccf56ec184a4e3f30397
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260937"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="e8ae9-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="e8ae9-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="e8ae9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e8ae9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8ae9-105">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="e8ae9-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="e8ae9-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8ae9-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8ae9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8ae9-107">Properties</span></span>
|<span data-ttu-id="e8ae9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8ae9-108">Property</span></span>|<span data-ttu-id="e8ae9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e8ae9-109">Type</span></span>|<span data-ttu-id="e8ae9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e8ae9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8ae9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="e8ae9-111">displayName</span></span>|<span data-ttu-id="e8ae9-112">String</span><span class="sxs-lookup"><span data-stu-id="e8ae9-112">String</span></span>|<span data-ttu-id="e8ae9-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8ae9-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="e8ae9-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="e8ae9-114">bundleID</span></span>|<span data-ttu-id="e8ae9-115">String</span><span class="sxs-lookup"><span data-stu-id="e8ae9-115">String</span></span>|<span data-ttu-id="e8ae9-116">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="e8ae9-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8ae9-117">Связи</span><span class="sxs-lookup"><span data-stu-id="e8ae9-117">Relationships</span></span>
<span data-ttu-id="e8ae9-118">Нет</span><span class="sxs-lookup"><span data-stu-id="e8ae9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e8ae9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8ae9-119">JSON Representation</span></span>
<span data-ttu-id="e8ae9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8ae9-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



