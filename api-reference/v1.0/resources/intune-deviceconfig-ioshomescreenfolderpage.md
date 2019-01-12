---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0417e7109d95c87083034fa9f7522c0f81dbfb99
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965854"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="51179-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="51179-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="51179-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="51179-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51179-105">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="51179-105">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="51179-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="51179-106">Properties</span></span>
|<span data-ttu-id="51179-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="51179-107">Property</span></span>|<span data-ttu-id="51179-108">Тип</span><span class="sxs-lookup"><span data-stu-id="51179-108">Type</span></span>|<span data-ttu-id="51179-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51179-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51179-110">displayName</span><span class="sxs-lookup"><span data-stu-id="51179-110">displayName</span></span>|<span data-ttu-id="51179-111">String</span><span class="sxs-lookup"><span data-stu-id="51179-111">String</span></span>|<span data-ttu-id="51179-112">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="51179-112">Name of the folder page</span></span>|
|<span data-ttu-id="51179-113">apps</span><span class="sxs-lookup"><span data-stu-id="51179-113">apps</span></span>|<span data-ttu-id="51179-114">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="51179-114">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="51179-115">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="51179-115">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="51179-116">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="51179-116">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51179-117">Связи</span><span class="sxs-lookup"><span data-stu-id="51179-117">Relationships</span></span>
<span data-ttu-id="51179-118">Нет</span><span class="sxs-lookup"><span data-stu-id="51179-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51179-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51179-119">JSON Representation</span></span>
<span data-ttu-id="51179-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51179-120">Here is a JSON representation of the resource.</span></span>
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



