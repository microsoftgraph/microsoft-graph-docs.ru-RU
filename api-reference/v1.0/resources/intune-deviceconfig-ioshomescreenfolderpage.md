---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f00c67b7a0679d92ef6aac78bc0317e461dcd2f9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255495"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="5ed12-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="5ed12-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="5ed12-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="5ed12-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ed12-105">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="5ed12-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="5ed12-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="5ed12-106">Properties</span></span>
|<span data-ttu-id="5ed12-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="5ed12-107">Property</span></span>|<span data-ttu-id="5ed12-108">Тип</span><span class="sxs-lookup"><span data-stu-id="5ed12-108">Type</span></span>|<span data-ttu-id="5ed12-109">Описание</span><span class="sxs-lookup"><span data-stu-id="5ed12-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ed12-110">displayName</span><span class="sxs-lookup"><span data-stu-id="5ed12-110">displayName</span></span>|<span data-ttu-id="5ed12-111">String</span><span class="sxs-lookup"><span data-stu-id="5ed12-111">String</span></span>|<span data-ttu-id="5ed12-112">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="5ed12-112">Name of the folder page</span></span>|
|<span data-ttu-id="5ed12-113">apps</span><span class="sxs-lookup"><span data-stu-id="5ed12-113">apps</span></span>|<span data-ttu-id="5ed12-114">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="5ed12-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="5ed12-115">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="5ed12-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="5ed12-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="5ed12-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ed12-117">Связи</span><span class="sxs-lookup"><span data-stu-id="5ed12-117">Relationships</span></span>
<span data-ttu-id="5ed12-118">Нет</span><span class="sxs-lookup"><span data-stu-id="5ed12-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5ed12-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5ed12-119">JSON Representation</span></span>
<span data-ttu-id="5ed12-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5ed12-120">Here is a JSON representation of the resource.</span></span>
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



