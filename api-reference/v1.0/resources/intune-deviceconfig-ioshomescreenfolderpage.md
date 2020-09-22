---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e60e0365656a9b1dee0bb78022edeaeef7e5e6f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47984434"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="06454-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="06454-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="06454-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06454-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="06454-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="06454-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06454-106">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="06454-106">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="06454-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="06454-107">Properties</span></span>
|<span data-ttu-id="06454-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="06454-108">Property</span></span>|<span data-ttu-id="06454-109">Тип</span><span class="sxs-lookup"><span data-stu-id="06454-109">Type</span></span>|<span data-ttu-id="06454-110">Описание</span><span class="sxs-lookup"><span data-stu-id="06454-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06454-111">displayName</span><span class="sxs-lookup"><span data-stu-id="06454-111">displayName</span></span>|<span data-ttu-id="06454-112">String</span><span class="sxs-lookup"><span data-stu-id="06454-112">String</span></span>|<span data-ttu-id="06454-113">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="06454-113">Name of the folder page</span></span>|
|<span data-ttu-id="06454-114">apps</span><span class="sxs-lookup"><span data-stu-id="06454-114">apps</span></span>|<span data-ttu-id="06454-115">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="06454-115">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="06454-116">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="06454-116">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="06454-117">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="06454-117">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="06454-118">Связи</span><span class="sxs-lookup"><span data-stu-id="06454-118">Relationships</span></span>
<span data-ttu-id="06454-119">Нет</span><span class="sxs-lookup"><span data-stu-id="06454-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06454-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="06454-120">JSON Representation</span></span>
<span data-ttu-id="06454-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="06454-121">Here is a JSON representation of the resource.</span></span>
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









