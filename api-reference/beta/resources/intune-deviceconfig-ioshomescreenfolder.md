---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1cf7ef74b12efbe81503ad46f1a9c766fcc996c5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357042"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="d98f9-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="d98f9-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="d98f9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d98f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d98f9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d98f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d98f9-106">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="d98f9-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="d98f9-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d98f9-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d98f9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d98f9-108">Properties</span></span>
|<span data-ttu-id="d98f9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d98f9-109">Property</span></span>|<span data-ttu-id="d98f9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d98f9-110">Type</span></span>|<span data-ttu-id="d98f9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d98f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d98f9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d98f9-112">displayName</span></span>|<span data-ttu-id="d98f9-113">String</span><span class="sxs-lookup"><span data-stu-id="d98f9-113">String</span></span>|<span data-ttu-id="d98f9-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d98f9-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d98f9-115">pages</span><span class="sxs-lookup"><span data-stu-id="d98f9-115">pages</span></span>|<span data-ttu-id="d98f9-116">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="d98f9-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="d98f9-117">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="d98f9-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="d98f9-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d98f9-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d98f9-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="d98f9-119">Relationships</span></span>
<span data-ttu-id="d98f9-120">Нет</span><span class="sxs-lookup"><span data-stu-id="d98f9-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d98f9-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d98f9-121">JSON Representation</span></span>
<span data-ttu-id="d98f9-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d98f9-122">Here is a JSON representation of the resource.</span></span>
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



