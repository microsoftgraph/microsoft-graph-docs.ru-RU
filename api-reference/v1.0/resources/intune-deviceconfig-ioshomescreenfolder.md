---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 59d4fe30fd274cd1051de50e225f449570de38ed
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410702"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="f23dd-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="f23dd-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="f23dd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f23dd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f23dd-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f23dd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f23dd-106">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="f23dd-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="f23dd-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="f23dd-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f23dd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f23dd-108">Properties</span></span>
|<span data-ttu-id="f23dd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f23dd-109">Property</span></span>|<span data-ttu-id="f23dd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f23dd-110">Type</span></span>|<span data-ttu-id="f23dd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f23dd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23dd-112">displayName</span><span class="sxs-lookup"><span data-stu-id="f23dd-112">displayName</span></span>|<span data-ttu-id="f23dd-113">String</span><span class="sxs-lookup"><span data-stu-id="f23dd-113">String</span></span>|<span data-ttu-id="f23dd-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="f23dd-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="f23dd-115">pages</span><span class="sxs-lookup"><span data-stu-id="f23dd-115">pages</span></span>|<span data-ttu-id="f23dd-116">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="f23dd-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="f23dd-117">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="f23dd-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="f23dd-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="f23dd-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f23dd-119">Связи</span><span class="sxs-lookup"><span data-stu-id="f23dd-119">Relationships</span></span>
<span data-ttu-id="f23dd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="f23dd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f23dd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f23dd-121">JSON Representation</span></span>
<span data-ttu-id="f23dd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f23dd-122">Here is a JSON representation of the resource.</span></span>
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







