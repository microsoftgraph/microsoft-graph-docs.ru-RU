---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83b9c116f31a8f129394e618cf86e3382c1d528a
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359123"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="b4678-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="b4678-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="b4678-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b4678-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4678-105">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="b4678-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="b4678-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4678-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b4678-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b4678-107">Properties</span></span>
|<span data-ttu-id="b4678-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b4678-108">Property</span></span>|<span data-ttu-id="b4678-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b4678-109">Type</span></span>|<span data-ttu-id="b4678-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b4678-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4678-111">displayName</span><span class="sxs-lookup"><span data-stu-id="b4678-111">displayName</span></span>|<span data-ttu-id="b4678-112">String</span><span class="sxs-lookup"><span data-stu-id="b4678-112">String</span></span>|<span data-ttu-id="b4678-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b4678-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="b4678-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="b4678-114">bundleID</span></span>|<span data-ttu-id="b4678-115">String</span><span class="sxs-lookup"><span data-stu-id="b4678-115">String</span></span>|<span data-ttu-id="b4678-116">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="b4678-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="b4678-117">Связи</span><span class="sxs-lookup"><span data-stu-id="b4678-117">Relationships</span></span>
<span data-ttu-id="b4678-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b4678-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b4678-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b4678-119">JSON Representation</span></span>
<span data-ttu-id="b4678-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b4678-120">Here is a JSON representation of the resource.</span></span>
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




