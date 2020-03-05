---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dab4cc8829a5d3970778465b404b7fb29a4d0556
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529906"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="07e03-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="07e03-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="07e03-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="07e03-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07e03-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07e03-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07e03-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07e03-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07e03-107">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="07e03-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="07e03-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07e03-108">Properties</span></span>
|<span data-ttu-id="07e03-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="07e03-109">Property</span></span>|<span data-ttu-id="07e03-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07e03-110">Type</span></span>|<span data-ttu-id="07e03-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07e03-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07e03-112">displayName</span><span class="sxs-lookup"><span data-stu-id="07e03-112">displayName</span></span>|<span data-ttu-id="07e03-113">String</span><span class="sxs-lookup"><span data-stu-id="07e03-113">String</span></span>|<span data-ttu-id="07e03-114">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="07e03-114">Name of the folder page</span></span>|
|<span data-ttu-id="07e03-115">apps</span><span class="sxs-lookup"><span data-stu-id="07e03-115">apps</span></span>|<span data-ttu-id="07e03-116">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="07e03-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="07e03-117">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="07e03-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="07e03-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="07e03-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07e03-119">Связи</span><span class="sxs-lookup"><span data-stu-id="07e03-119">Relationships</span></span>
<span data-ttu-id="07e03-120">Нет</span><span class="sxs-lookup"><span data-stu-id="07e03-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07e03-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07e03-121">JSON Representation</span></span>
<span data-ttu-id="07e03-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07e03-122">Here is a JSON representation of the resource.</span></span>
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



