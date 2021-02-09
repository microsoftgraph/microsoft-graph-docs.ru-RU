---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений и веб-клипов на домашнем экране.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7ad090d7e5a01eaf3dda10c6d9edd5cfafacb1a2
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161819"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="b830d-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="b830d-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="b830d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b830d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b830d-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b830d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b830d-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b830d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b830d-107">Папка, содержащая страницы приложений и веб-клипов на домашнем экране.</span><span class="sxs-lookup"><span data-stu-id="b830d-107">A folder containing pages of apps and web clips on the Home Screen.</span></span>


<span data-ttu-id="b830d-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b830d-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b830d-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b830d-109">Properties</span></span>
|<span data-ttu-id="b830d-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b830d-110">Property</span></span>|<span data-ttu-id="b830d-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b830d-111">Type</span></span>|<span data-ttu-id="b830d-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b830d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b830d-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b830d-113">displayName</span></span>|<span data-ttu-id="b830d-114">String</span><span class="sxs-lookup"><span data-stu-id="b830d-114">String</span></span>|<span data-ttu-id="b830d-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b830d-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="b830d-116">pages</span><span class="sxs-lookup"><span data-stu-id="b830d-116">pages</span></span>|<span data-ttu-id="b830d-117">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="b830d-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="b830d-118">Страницы значков макета домашнего экрана, которые должны быть приложениями или веб-клипами.</span><span class="sxs-lookup"><span data-stu-id="b830d-118">Pages of Home Screen Layout Icons which must be applications or web clips.</span></span> <span data-ttu-id="b830d-119">Эта коллекция может содержать не более 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="b830d-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b830d-120">Связи</span><span class="sxs-lookup"><span data-stu-id="b830d-120">Relationships</span></span>
<span data-ttu-id="b830d-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b830d-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b830d-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b830d-122">JSON Representation</span></span>
<span data-ttu-id="b830d-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b830d-123">Here is a JSON representation of the resource.</span></span>
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
          "bundleID": "String",
          "isWebClip": true
        }
      ]
    }
  ]
}
```




