---
title: Тип ресурса iosHomeScreenFolderPage
description: Папка, содержащая приложения с начального экрана
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1fa9462f8fb0640584515d1c209abd03de0e6200
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424177"
---
# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="37de0-103">Тип ресурса iosHomeScreenFolderPage</span><span class="sxs-lookup"><span data-stu-id="37de0-103">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="37de0-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="37de0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37de0-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="37de0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37de0-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="37de0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37de0-107">Папка, содержащая приложения с начального экрана</span><span class="sxs-lookup"><span data-stu-id="37de0-107">A folder containing apps on the Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="37de0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="37de0-108">Properties</span></span>
|<span data-ttu-id="37de0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="37de0-109">Property</span></span>|<span data-ttu-id="37de0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="37de0-110">Type</span></span>|<span data-ttu-id="37de0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="37de0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37de0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="37de0-112">displayName</span></span>|<span data-ttu-id="37de0-113">String</span><span class="sxs-lookup"><span data-stu-id="37de0-113">String</span></span>|<span data-ttu-id="37de0-114">Имя страницы папки</span><span class="sxs-lookup"><span data-stu-id="37de0-114">Name of the folder page</span></span>|
|<span data-ttu-id="37de0-115">apps</span><span class="sxs-lookup"><span data-stu-id="37de0-115">apps</span></span>|<span data-ttu-id="37de0-116">Коллекция [iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md)</span><span class="sxs-lookup"><span data-stu-id="37de0-116">[iosHomeScreenApp](../resources/intune-deviceconfig-ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="37de0-117">Список приложений, которые отображаются на странице в папке.</span><span class="sxs-lookup"><span data-stu-id="37de0-117">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="37de0-118">Эта коллекция может включать до 500 элементов.</span><span class="sxs-lookup"><span data-stu-id="37de0-118">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37de0-119">Связи</span><span class="sxs-lookup"><span data-stu-id="37de0-119">Relationships</span></span>
<span data-ttu-id="37de0-120">Нет</span><span class="sxs-lookup"><span data-stu-id="37de0-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37de0-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="37de0-121">JSON Representation</span></span>
<span data-ttu-id="37de0-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="37de0-122">Here is a JSON representation of the resource.</span></span>
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




