---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
ms.openlocfilehash: ff749f7166da2d20bfd632e0c595b33f7b1e9fad
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027152"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="d613d-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="d613d-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="d613d-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d613d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d613d-105">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="d613d-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="d613d-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d613d-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d613d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d613d-107">Properties</span></span>
|<span data-ttu-id="d613d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d613d-108">Property</span></span>|<span data-ttu-id="d613d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d613d-109">Type</span></span>|<span data-ttu-id="d613d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d613d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d613d-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d613d-111">displayName</span></span>|<span data-ttu-id="d613d-112">String</span><span class="sxs-lookup"><span data-stu-id="d613d-112">String</span></span>|<span data-ttu-id="d613d-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="d613d-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="d613d-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="d613d-114">bundleID</span></span>|<span data-ttu-id="d613d-115">String</span><span class="sxs-lookup"><span data-stu-id="d613d-115">String</span></span>|<span data-ttu-id="d613d-116">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="d613d-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="d613d-117">Связи</span><span class="sxs-lookup"><span data-stu-id="d613d-117">Relationships</span></span>
<span data-ttu-id="d613d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d613d-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d613d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d613d-119">JSON Representation</span></span>
<span data-ttu-id="d613d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d613d-120">Here is a JSON representation of the resource.</span></span>
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



