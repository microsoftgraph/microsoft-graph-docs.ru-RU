---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcc90e774f8d032d46968fc4f751923bcc52e559
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412326"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="958f5-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="958f5-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="958f5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="958f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="958f5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="958f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="958f5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="958f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="958f5-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="958f5-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="958f5-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="958f5-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="958f5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="958f5-109">Properties</span></span>
|<span data-ttu-id="958f5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="958f5-110">Property</span></span>|<span data-ttu-id="958f5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="958f5-111">Type</span></span>|<span data-ttu-id="958f5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="958f5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="958f5-113">displayName</span><span class="sxs-lookup"><span data-stu-id="958f5-113">displayName</span></span>|<span data-ttu-id="958f5-114">String</span><span class="sxs-lookup"><span data-stu-id="958f5-114">String</span></span>|<span data-ttu-id="958f5-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="958f5-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="958f5-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="958f5-116">bundleID</span></span>|<span data-ttu-id="958f5-117">String</span><span class="sxs-lookup"><span data-stu-id="958f5-117">String</span></span>|<span data-ttu-id="958f5-118">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="958f5-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="958f5-119">Связи</span><span class="sxs-lookup"><span data-stu-id="958f5-119">Relationships</span></span>
<span data-ttu-id="958f5-120">Нет</span><span class="sxs-lookup"><span data-stu-id="958f5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="958f5-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="958f5-121">JSON Representation</span></span>
<span data-ttu-id="958f5-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="958f5-122">Here is a JSON representation of the resource.</span></span>
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




