---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bb2ea3cb1a183af0f437a7a128331084634cca4b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410639"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="49a60-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="49a60-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="49a60-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49a60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49a60-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="49a60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49a60-106">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="49a60-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="49a60-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="49a60-107">Properties</span></span>
|<span data-ttu-id="49a60-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="49a60-108">Property</span></span>|<span data-ttu-id="49a60-109">Тип</span><span class="sxs-lookup"><span data-stu-id="49a60-109">Type</span></span>|<span data-ttu-id="49a60-110">Описание</span><span class="sxs-lookup"><span data-stu-id="49a60-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49a60-111">displayName</span><span class="sxs-lookup"><span data-stu-id="49a60-111">displayName</span></span>|<span data-ttu-id="49a60-112">String</span><span class="sxs-lookup"><span data-stu-id="49a60-112">String</span></span>|<span data-ttu-id="49a60-113">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="49a60-113">Name of the folder page</span></span>|
|<span data-ttu-id="49a60-114">apps</span><span class="sxs-lookup"><span data-stu-id="49a60-114">apps</span></span>|<span data-ttu-id="49a60-115">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="49a60-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="49a60-116">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="49a60-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="49a60-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="49a60-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="49a60-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="49a60-118">Relationships</span></span>
<span data-ttu-id="49a60-119">Нет</span><span class="sxs-lookup"><span data-stu-id="49a60-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49a60-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="49a60-120">JSON Representation</span></span>
<span data-ttu-id="49a60-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="49a60-121">Here is a JSON representation of the resource.</span></span>
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







