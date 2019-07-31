---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2211b8424501407ceaf4cf612820f16600757d64
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36001266"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="0ac0b-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="0ac0b-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="0ac0b-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0ac0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0ac0b-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0ac0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ac0b-106">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="0ac0b-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="0ac0b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ac0b-107">Properties</span></span>
|<span data-ttu-id="0ac0b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ac0b-108">Property</span></span>|<span data-ttu-id="0ac0b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="0ac0b-109">Type</span></span>|<span data-ttu-id="0ac0b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0ac0b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ac0b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac0b-111">displayName</span></span>|<span data-ttu-id="0ac0b-112">String</span><span class="sxs-lookup"><span data-stu-id="0ac0b-112">String</span></span>|<span data-ttu-id="0ac0b-113">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="0ac0b-113">Name of the folder page</span></span>|
|<span data-ttu-id="0ac0b-114">apps</span><span class="sxs-lookup"><span data-stu-id="0ac0b-114">apps</span></span>|<span data-ttu-id="0ac0b-115">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="0ac0b-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="0ac0b-116">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="0ac0b-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="0ac0b-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="0ac0b-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ac0b-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="0ac0b-118">Relationships</span></span>
<span data-ttu-id="0ac0b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="0ac0b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0ac0b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ac0b-120">JSON Representation</span></span>
<span data-ttu-id="0ac0b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ac0b-121">Here is a JSON representation of the resource.</span></span>
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





