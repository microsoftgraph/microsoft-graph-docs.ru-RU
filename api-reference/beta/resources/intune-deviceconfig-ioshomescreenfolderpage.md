---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 93fca952cfda7bf1e49c17a3fe71b3a62384d0e6
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791578"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="40f66-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="40f66-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="40f66-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="40f66-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40f66-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="40f66-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40f66-106">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="40f66-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="40f66-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="40f66-107">Properties</span></span>
|<span data-ttu-id="40f66-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="40f66-108">Property</span></span>|<span data-ttu-id="40f66-109">Тип</span><span class="sxs-lookup"><span data-stu-id="40f66-109">Type</span></span>|<span data-ttu-id="40f66-110">Описание</span><span class="sxs-lookup"><span data-stu-id="40f66-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40f66-111">displayName</span><span class="sxs-lookup"><span data-stu-id="40f66-111">displayName</span></span>|<span data-ttu-id="40f66-112">String</span><span class="sxs-lookup"><span data-stu-id="40f66-112">String</span></span>|<span data-ttu-id="40f66-113">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="40f66-113">Name of the folder page</span></span>|
|<span data-ttu-id="40f66-114">apps</span><span class="sxs-lookup"><span data-stu-id="40f66-114">apps</span></span>|<span data-ttu-id="40f66-115">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="40f66-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="40f66-116">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="40f66-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="40f66-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="40f66-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="40f66-118">Связи</span><span class="sxs-lookup"><span data-stu-id="40f66-118">Relationships</span></span>
<span data-ttu-id="40f66-119">Нет</span><span class="sxs-lookup"><span data-stu-id="40f66-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="40f66-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="40f66-120">JSON Representation</span></span>
<span data-ttu-id="40f66-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="40f66-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```



