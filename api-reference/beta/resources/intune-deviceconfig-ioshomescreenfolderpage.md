---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d8d1765cbad7f904c994aac1872f40231fc525c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521665"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="24d6f-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="24d6f-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="24d6f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="24d6f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24d6f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="24d6f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24d6f-106">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="24d6f-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="24d6f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="24d6f-107">Properties</span></span>
|<span data-ttu-id="24d6f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="24d6f-108">Property</span></span>|<span data-ttu-id="24d6f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="24d6f-109">Type</span></span>|<span data-ttu-id="24d6f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="24d6f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24d6f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="24d6f-111">displayName</span></span>|<span data-ttu-id="24d6f-112">String</span><span class="sxs-lookup"><span data-stu-id="24d6f-112">String</span></span>|<span data-ttu-id="24d6f-113">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="24d6f-113">Name of the folder page</span></span>|
|<span data-ttu-id="24d6f-114">apps</span><span class="sxs-lookup"><span data-stu-id="24d6f-114">apps</span></span>|<span data-ttu-id="24d6f-115">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="24d6f-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="24d6f-116">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="24d6f-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="24d6f-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="24d6f-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24d6f-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="24d6f-118">Relationships</span></span>
<span data-ttu-id="24d6f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="24d6f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24d6f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24d6f-120">JSON Representation</span></span>
<span data-ttu-id="24d6f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24d6f-121">Here is a JSON representation of the resource.</span></span>
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





