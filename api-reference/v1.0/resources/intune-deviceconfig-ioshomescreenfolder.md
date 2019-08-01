---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a22b20049c886b7cb1de2f7737b269fbd411749
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031523"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="77ea9-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="77ea9-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="77ea9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="77ea9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77ea9-105">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="77ea9-105">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="77ea9-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="77ea9-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="77ea9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="77ea9-107">Properties</span></span>
|<span data-ttu-id="77ea9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="77ea9-108">Property</span></span>|<span data-ttu-id="77ea9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="77ea9-109">Type</span></span>|<span data-ttu-id="77ea9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="77ea9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77ea9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="77ea9-111">displayName</span></span>|<span data-ttu-id="77ea9-112">String</span><span class="sxs-lookup"><span data-stu-id="77ea9-112">String</span></span>|<span data-ttu-id="77ea9-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="77ea9-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="77ea9-114">pages</span><span class="sxs-lookup"><span data-stu-id="77ea9-114">pages</span></span>|<span data-ttu-id="77ea9-115">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="77ea9-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="77ea9-116">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="77ea9-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="77ea9-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="77ea9-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77ea9-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="77ea9-118">Relationships</span></span>
<span data-ttu-id="77ea9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="77ea9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77ea9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="77ea9-120">JSON Representation</span></span>
<span data-ttu-id="77ea9-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="77ea9-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
  "displayName": "String",
  "pages": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
      "displayName": "String",
      "apps": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenApp",
          "displayName": "String",
          "bundleID": "String"
        }
      ]
    }
  ]
}
```



