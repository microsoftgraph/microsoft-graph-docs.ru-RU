---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d27d632050a288966e5f1596e94243b08b40726e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981751"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="fe3a2-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="fe3a2-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="fe3a2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fe3a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe3a2-105">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="fe3a2-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="fe3a2-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe3a2-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fe3a2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe3a2-107">Properties</span></span>
|<span data-ttu-id="fe3a2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe3a2-108">Property</span></span>|<span data-ttu-id="fe3a2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fe3a2-109">Type</span></span>|<span data-ttu-id="fe3a2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe3a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe3a2-111">displayName</span><span class="sxs-lookup"><span data-stu-id="fe3a2-111">displayName</span></span>|<span data-ttu-id="fe3a2-112">String</span><span class="sxs-lookup"><span data-stu-id="fe3a2-112">String</span></span>|<span data-ttu-id="fe3a2-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="fe3a2-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="fe3a2-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="fe3a2-114">bundleID</span></span>|<span data-ttu-id="fe3a2-115">String</span><span class="sxs-lookup"><span data-stu-id="fe3a2-115">String</span></span>|<span data-ttu-id="fe3a2-116">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="fe3a2-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe3a2-117">Связи</span><span class="sxs-lookup"><span data-stu-id="fe3a2-117">Relationships</span></span>
<span data-ttu-id="fe3a2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fe3a2-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fe3a2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe3a2-119">JSON Representation</span></span>
<span data-ttu-id="fe3a2-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe3a2-120">Here is a JSON representation of the resource.</span></span>
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



