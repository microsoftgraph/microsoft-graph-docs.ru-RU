---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc4e94071e7b81fab82044f65da809f7b17e5b3f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028219"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="af19b-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="af19b-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="af19b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af19b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af19b-105">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="af19b-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="af19b-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="af19b-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="af19b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="af19b-107">Properties</span></span>
|<span data-ttu-id="af19b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="af19b-108">Property</span></span>|<span data-ttu-id="af19b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="af19b-109">Type</span></span>|<span data-ttu-id="af19b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af19b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af19b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="af19b-111">displayName</span></span>|<span data-ttu-id="af19b-112">String</span><span class="sxs-lookup"><span data-stu-id="af19b-112">String</span></span>|<span data-ttu-id="af19b-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="af19b-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="af19b-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="af19b-114">bundleID</span></span>|<span data-ttu-id="af19b-115">String</span><span class="sxs-lookup"><span data-stu-id="af19b-115">String</span></span>|<span data-ttu-id="af19b-116">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="af19b-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="af19b-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="af19b-117">Relationships</span></span>
<span data-ttu-id="af19b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="af19b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af19b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af19b-119">JSON Representation</span></span>
<span data-ttu-id="af19b-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af19b-120">Here is a JSON representation of the resource.</span></span>
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



