---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 36ea4a00b9310623027179e1d6d2e1c64888c470
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407510"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="267b6-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="267b6-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="267b6-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="267b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="267b6-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="267b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="267b6-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="267b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="267b6-107">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="267b6-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="267b6-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="267b6-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="267b6-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="267b6-109">Properties</span></span>
|<span data-ttu-id="267b6-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="267b6-110">Property</span></span>|<span data-ttu-id="267b6-111">Тип</span><span class="sxs-lookup"><span data-stu-id="267b6-111">Type</span></span>|<span data-ttu-id="267b6-112">Описание</span><span class="sxs-lookup"><span data-stu-id="267b6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="267b6-113">displayName</span><span class="sxs-lookup"><span data-stu-id="267b6-113">displayName</span></span>|<span data-ttu-id="267b6-114">String</span><span class="sxs-lookup"><span data-stu-id="267b6-114">String</span></span>|<span data-ttu-id="267b6-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="267b6-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="267b6-116">pages</span><span class="sxs-lookup"><span data-stu-id="267b6-116">pages</span></span>|<span data-ttu-id="267b6-117">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="267b6-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="267b6-118">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="267b6-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="267b6-119">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="267b6-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="267b6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="267b6-120">Relationships</span></span>
<span data-ttu-id="267b6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="267b6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="267b6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="267b6-122">JSON Representation</span></span>
<span data-ttu-id="267b6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="267b6-123">Here is a JSON representation of the resource.</span></span>
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




