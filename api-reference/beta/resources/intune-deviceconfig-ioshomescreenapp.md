---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eb9d3dcd32834167ab89a1e62311942a542f74ac
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791592"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="2bed2-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="2bed2-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="2bed2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2bed2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bed2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2bed2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bed2-106">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="2bed2-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="2bed2-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="2bed2-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2bed2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2bed2-108">Properties</span></span>
|<span data-ttu-id="2bed2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2bed2-109">Property</span></span>|<span data-ttu-id="2bed2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2bed2-110">Type</span></span>|<span data-ttu-id="2bed2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2bed2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bed2-112">displayName</span><span class="sxs-lookup"><span data-stu-id="2bed2-112">displayName</span></span>|<span data-ttu-id="2bed2-113">String</span><span class="sxs-lookup"><span data-stu-id="2bed2-113">String</span></span>|<span data-ttu-id="2bed2-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="2bed2-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="2bed2-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="2bed2-115">bundleID</span></span>|<span data-ttu-id="2bed2-116">String</span><span class="sxs-lookup"><span data-stu-id="2bed2-116">String</span></span>|<span data-ttu-id="2bed2-117">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="2bed2-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bed2-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2bed2-118">Relationships</span></span>
<span data-ttu-id="2bed2-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2bed2-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bed2-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2bed2-120">JSON Representation</span></span>
<span data-ttu-id="2bed2-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2bed2-121">Here is a JSON representation of the resource.</span></span>
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



