---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6e4934565255e364012eedb54044b37281c1641
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786583"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="1c520-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="1c520-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="1c520-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1c520-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1c520-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1c520-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1c520-106">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="1c520-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="1c520-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c520-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1c520-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1c520-108">Properties</span></span>
|<span data-ttu-id="1c520-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1c520-109">Property</span></span>|<span data-ttu-id="1c520-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1c520-110">Type</span></span>|<span data-ttu-id="1c520-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1c520-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1c520-112">displayName</span><span class="sxs-lookup"><span data-stu-id="1c520-112">displayName</span></span>|<span data-ttu-id="1c520-113">String</span><span class="sxs-lookup"><span data-stu-id="1c520-113">String</span></span>|<span data-ttu-id="1c520-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="1c520-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="1c520-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="1c520-115">bundleID</span></span>|<span data-ttu-id="1c520-116">String</span><span class="sxs-lookup"><span data-stu-id="1c520-116">String</span></span>|<span data-ttu-id="1c520-117">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="1c520-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="1c520-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="1c520-118">Relationships</span></span>
<span data-ttu-id="1c520-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1c520-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1c520-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1c520-120">JSON Representation</span></span>
<span data-ttu-id="1c520-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1c520-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```





