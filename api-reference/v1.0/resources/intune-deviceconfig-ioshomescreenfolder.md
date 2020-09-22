---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e68172006eac3417bb87424cce19f0e2be9b78a1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984441"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="72485-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="72485-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="72485-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72485-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72485-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72485-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72485-106">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="72485-106">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="72485-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="72485-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="72485-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="72485-108">Properties</span></span>
|<span data-ttu-id="72485-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="72485-109">Property</span></span>|<span data-ttu-id="72485-110">Тип</span><span class="sxs-lookup"><span data-stu-id="72485-110">Type</span></span>|<span data-ttu-id="72485-111">Описание</span><span class="sxs-lookup"><span data-stu-id="72485-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72485-112">displayName</span><span class="sxs-lookup"><span data-stu-id="72485-112">displayName</span></span>|<span data-ttu-id="72485-113">String</span><span class="sxs-lookup"><span data-stu-id="72485-113">String</span></span>|<span data-ttu-id="72485-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="72485-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="72485-115">pages</span><span class="sxs-lookup"><span data-stu-id="72485-115">pages</span></span>|<span data-ttu-id="72485-116">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="72485-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="72485-117">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="72485-117">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="72485-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="72485-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72485-119">Связи</span><span class="sxs-lookup"><span data-stu-id="72485-119">Relationships</span></span>
<span data-ttu-id="72485-120">Нет</span><span class="sxs-lookup"><span data-stu-id="72485-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72485-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72485-121">JSON Representation</span></span>
<span data-ttu-id="72485-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72485-122">Here is a JSON representation of the resource.</span></span>
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









