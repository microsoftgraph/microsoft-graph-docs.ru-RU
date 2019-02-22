---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8afb80b9130356671d80e5ec52f96bf74ed53d7e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153741"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="5d074-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="5d074-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="5d074-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5d074-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d074-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5d074-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d074-106">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="5d074-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="5d074-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="5d074-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5d074-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d074-108">Properties</span></span>
|<span data-ttu-id="5d074-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d074-109">Property</span></span>|<span data-ttu-id="5d074-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5d074-110">Type</span></span>|<span data-ttu-id="5d074-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5d074-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d074-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5d074-112">displayName</span></span>|<span data-ttu-id="5d074-113">String</span><span class="sxs-lookup"><span data-stu-id="5d074-113">String</span></span>|<span data-ttu-id="5d074-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="5d074-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="5d074-115">pages</span><span class="sxs-lookup"><span data-stu-id="5d074-115">pages</span></span>|<span data-ttu-id="5d074-116">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="5d074-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="5d074-117">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="5d074-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="5d074-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5d074-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d074-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5d074-119">Relationships</span></span>
<span data-ttu-id="5d074-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5d074-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d074-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5d074-121">JSON Representation</span></span>
<span data-ttu-id="5d074-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d074-122">Here is a JSON representation of the resource.</span></span>
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




