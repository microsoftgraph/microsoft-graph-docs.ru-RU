---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 76a8237442e0e807e0a1383c8032cf4e6361516e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028212"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="d67ee-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="d67ee-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="d67ee-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d67ee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d67ee-105">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="d67ee-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="d67ee-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="d67ee-106">Properties</span></span>
|<span data-ttu-id="d67ee-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="d67ee-107">Property</span></span>|<span data-ttu-id="d67ee-108">Тип</span><span class="sxs-lookup"><span data-stu-id="d67ee-108">Type</span></span>|<span data-ttu-id="d67ee-109">Описание</span><span class="sxs-lookup"><span data-stu-id="d67ee-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d67ee-110">displayName</span><span class="sxs-lookup"><span data-stu-id="d67ee-110">displayName</span></span>|<span data-ttu-id="d67ee-111">String</span><span class="sxs-lookup"><span data-stu-id="d67ee-111">String</span></span>|<span data-ttu-id="d67ee-112">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="d67ee-112">Name of the folder page</span></span>|
|<span data-ttu-id="d67ee-113">apps</span><span class="sxs-lookup"><span data-stu-id="d67ee-113">apps</span></span>|<span data-ttu-id="d67ee-114">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="d67ee-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="d67ee-115">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="d67ee-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="d67ee-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="d67ee-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d67ee-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="d67ee-117">Relationships</span></span>
<span data-ttu-id="d67ee-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d67ee-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d67ee-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d67ee-119">JSON Representation</span></span>
<span data-ttu-id="d67ee-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d67ee-120">Here is a JSON representation of the resource.</span></span>
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



