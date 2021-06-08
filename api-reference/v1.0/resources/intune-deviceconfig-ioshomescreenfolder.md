---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений и веб-клипы на домашнем экране.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4ee4d2f1119a7fb6c4318b2afd195518f4b8095b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760073"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="0d134-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="0d134-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="0d134-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d134-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d134-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0d134-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d134-106">Папка, содержащая страницы приложений и веб-клипы на домашнем экране.</span><span class="sxs-lookup"><span data-stu-id="0d134-106">A folder containing pages of apps and web clips on the Home Screen.</span></span>


<span data-ttu-id="0d134-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="0d134-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0d134-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0d134-108">Properties</span></span>
|<span data-ttu-id="0d134-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0d134-109">Property</span></span>|<span data-ttu-id="0d134-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0d134-110">Type</span></span>|<span data-ttu-id="0d134-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0d134-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d134-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0d134-112">displayName</span></span>|<span data-ttu-id="0d134-113">String</span><span class="sxs-lookup"><span data-stu-id="0d134-113">String</span></span>|<span data-ttu-id="0d134-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="0d134-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="0d134-115">pages</span><span class="sxs-lookup"><span data-stu-id="0d134-115">pages</span></span>|<span data-ttu-id="0d134-116">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="0d134-116">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="0d134-117">Страницы значков макета домашнего экрана, которые должны быть приложениями или веб-клипами.</span><span class="sxs-lookup"><span data-stu-id="0d134-117">Pages of Home Screen Layout Icons which must be applications or web clips.</span></span> <span data-ttu-id="0d134-118">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0d134-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d134-119">Связи</span><span class="sxs-lookup"><span data-stu-id="0d134-119">Relationships</span></span>
<span data-ttu-id="0d134-120">Нет</span><span class="sxs-lookup"><span data-stu-id="0d134-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d134-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0d134-121">JSON Representation</span></span>
<span data-ttu-id="0d134-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0d134-122">Here is a JSON representation of the resource.</span></span>
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




