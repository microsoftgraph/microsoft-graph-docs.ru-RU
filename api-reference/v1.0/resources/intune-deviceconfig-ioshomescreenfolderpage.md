---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f00c67b7a0679d92ef6aac78bc0317e461dcd2f9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554641"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="02725-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="02725-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="02725-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="02725-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02725-105">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="02725-105">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="02725-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="02725-106">Properties</span></span>
|<span data-ttu-id="02725-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="02725-107">Property</span></span>|<span data-ttu-id="02725-108">Тип</span><span class="sxs-lookup"><span data-stu-id="02725-108">Type</span></span>|<span data-ttu-id="02725-109">Описание</span><span class="sxs-lookup"><span data-stu-id="02725-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02725-110">displayName</span><span class="sxs-lookup"><span data-stu-id="02725-110">displayName</span></span>|<span data-ttu-id="02725-111">String</span><span class="sxs-lookup"><span data-stu-id="02725-111">String</span></span>|<span data-ttu-id="02725-112">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="02725-112">Name of the folder page</span></span>|
|<span data-ttu-id="02725-113">apps</span><span class="sxs-lookup"><span data-stu-id="02725-113">apps</span></span>|<span data-ttu-id="02725-114">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="02725-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="02725-115">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="02725-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="02725-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="02725-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="02725-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="02725-117">Relationships</span></span>
<span data-ttu-id="02725-118">Нет</span><span class="sxs-lookup"><span data-stu-id="02725-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="02725-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="02725-119">JSON Representation</span></span>
<span data-ttu-id="02725-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="02725-120">Here is a JSON representation of the resource.</span></span>
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



