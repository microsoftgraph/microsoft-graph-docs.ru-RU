---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6e35838ccd8a49bfe2609c29fe795bd21cfed723
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791585"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="5b834-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="5b834-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="5b834-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="5b834-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b834-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5b834-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b834-106">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="5b834-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="5b834-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="5b834-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5b834-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5b834-108">Properties</span></span>
|<span data-ttu-id="5b834-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5b834-109">Property</span></span>|<span data-ttu-id="5b834-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5b834-110">Type</span></span>|<span data-ttu-id="5b834-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5b834-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b834-112">displayName</span><span class="sxs-lookup"><span data-stu-id="5b834-112">displayName</span></span>|<span data-ttu-id="5b834-113">String</span><span class="sxs-lookup"><span data-stu-id="5b834-113">String</span></span>|<span data-ttu-id="5b834-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="5b834-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="5b834-115">pages</span><span class="sxs-lookup"><span data-stu-id="5b834-115">pages</span></span>|<span data-ttu-id="5b834-116">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="5b834-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="5b834-117">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="5b834-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="5b834-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5b834-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b834-119">Связи</span><span class="sxs-lookup"><span data-stu-id="5b834-119">Relationships</span></span>
<span data-ttu-id="5b834-120">Нет</span><span class="sxs-lookup"><span data-stu-id="5b834-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5b834-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5b834-121">JSON Representation</span></span>
<span data-ttu-id="5b834-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5b834-122">Here is a JSON representation of the resource.</span></span>
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



