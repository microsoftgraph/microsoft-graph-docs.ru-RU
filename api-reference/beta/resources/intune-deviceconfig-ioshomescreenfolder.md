---
title: Тип ресурса iosHomeScreenFolder
description: Папка, содержащая страницы приложений на начальном экране
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ad2f9cb0f5530aeffbc840f2e7f38b5e0fde59a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526362"
---
# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="31525-103">Тип ресурса iosHomeScreenFolder</span><span class="sxs-lookup"><span data-stu-id="31525-103">iosHomeScreenFolder resource type</span></span>

<span data-ttu-id="31525-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="31525-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="31525-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="31525-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31525-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="31525-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31525-107">Папка, содержащая страницы приложений на начальном экране</span><span class="sxs-lookup"><span data-stu-id="31525-107">A folder containing pages of apps on the Home Screen</span></span>


<span data-ttu-id="31525-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="31525-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="31525-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="31525-109">Properties</span></span>
|<span data-ttu-id="31525-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="31525-110">Property</span></span>|<span data-ttu-id="31525-111">Тип</span><span class="sxs-lookup"><span data-stu-id="31525-111">Type</span></span>|<span data-ttu-id="31525-112">Описание</span><span class="sxs-lookup"><span data-stu-id="31525-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31525-113">displayName</span><span class="sxs-lookup"><span data-stu-id="31525-113">displayName</span></span>|<span data-ttu-id="31525-114">String</span><span class="sxs-lookup"><span data-stu-id="31525-114">String</span></span>|<span data-ttu-id="31525-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="31525-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="31525-116">pages</span><span class="sxs-lookup"><span data-stu-id="31525-116">pages</span></span>|<span data-ttu-id="31525-117">Коллекция [iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md)</span><span class="sxs-lookup"><span data-stu-id="31525-117">[iosHomeScreenFolderPage](../resources/intune-deviceconfig-ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="31525-118">Страницы значков на начальном экране, которые должны относиться к типу приложения.</span><span class="sxs-lookup"><span data-stu-id="31525-118">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="31525-119">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="31525-119">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="31525-120">Связи</span><span class="sxs-lookup"><span data-stu-id="31525-120">Relationships</span></span>
<span data-ttu-id="31525-121">Нет</span><span class="sxs-lookup"><span data-stu-id="31525-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="31525-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31525-122">JSON Representation</span></span>
<span data-ttu-id="31525-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31525-123">Here is a JSON representation of the resource.</span></span>
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



