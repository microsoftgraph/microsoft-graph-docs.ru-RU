---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dd47562660f2941fbf722f92976817f310ff304f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930420"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="2082c-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="2082c-103">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="2082c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2082c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2082c-105">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="2082c-105">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="2082c-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="2082c-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2082c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2082c-107">Properties</span></span>
|<span data-ttu-id="2082c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2082c-108">Property</span></span>|<span data-ttu-id="2082c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2082c-109">Type</span></span>|<span data-ttu-id="2082c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2082c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2082c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="2082c-111">displayName</span></span>|<span data-ttu-id="2082c-112">String</span><span class="sxs-lookup"><span data-stu-id="2082c-112">String</span></span>|<span data-ttu-id="2082c-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="2082c-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="2082c-114">pages</span><span class="sxs-lookup"><span data-stu-id="2082c-114">pages</span></span>|<span data-ttu-id="2082c-115">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="2082c-115">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="2082c-116">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="2082c-116">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="2082c-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="2082c-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2082c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="2082c-118">Relationships</span></span>
<span data-ttu-id="2082c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="2082c-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2082c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2082c-120">JSON Representation</span></span>
<span data-ttu-id="2082c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2082c-121">Here is a JSON representation of the resource.</span></span>
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



