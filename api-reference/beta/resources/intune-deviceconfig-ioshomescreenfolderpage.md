---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7d50f83fb180df3d3c94e142854f7cce72955c38
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280433"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="bac29-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="bac29-103">iosHomeScreenFolderPage resource type</span></span>

<span data-ttu-id="bac29-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bac29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bac29-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bac29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bac29-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bac29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bac29-107">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="bac29-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="bac29-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bac29-108">Properties</span></span>
|<span data-ttu-id="bac29-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bac29-109">Property</span></span>|<span data-ttu-id="bac29-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bac29-110">Type</span></span>|<span data-ttu-id="bac29-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bac29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bac29-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bac29-112">displayName</span></span>|<span data-ttu-id="bac29-113">String</span><span class="sxs-lookup"><span data-stu-id="bac29-113">String</span></span>|<span data-ttu-id="bac29-114">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="bac29-114">Name of the folder page</span></span>|
|<span data-ttu-id="bac29-115">apps</span><span class="sxs-lookup"><span data-stu-id="bac29-115">apps</span></span>|<span data-ttu-id="bac29-116">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="bac29-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="bac29-117">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="bac29-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="bac29-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="bac29-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bac29-119">Связи</span><span class="sxs-lookup"><span data-stu-id="bac29-119">Relationships</span></span>
<span data-ttu-id="bac29-120">Нет</span><span class="sxs-lookup"><span data-stu-id="bac29-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bac29-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bac29-121">JSON Representation</span></span>
<span data-ttu-id="bac29-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bac29-122">Here is a JSON representation of the resource.</span></span>
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




