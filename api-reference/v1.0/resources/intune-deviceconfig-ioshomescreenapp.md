---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
ms.openlocfilehash: 68fe4e7b5a226422cc0aaf980ac7fb0421a9bfc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350374"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="c2464-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="c2464-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="c2464-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c2464-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2464-105">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="c2464-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="c2464-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2464-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c2464-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2464-107">Properties</span></span>
|<span data-ttu-id="c2464-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2464-108">Property</span></span>|<span data-ttu-id="c2464-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c2464-109">Type</span></span>|<span data-ttu-id="c2464-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c2464-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2464-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c2464-111">displayName</span></span>|<span data-ttu-id="c2464-112">String</span><span class="sxs-lookup"><span data-stu-id="c2464-112">String</span></span>|<span data-ttu-id="c2464-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="c2464-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="c2464-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="c2464-114">bundleID</span></span>|<span data-ttu-id="c2464-115">String</span><span class="sxs-lookup"><span data-stu-id="c2464-115">String</span></span>|<span data-ttu-id="c2464-116">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="c2464-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2464-117">Связи</span><span class="sxs-lookup"><span data-stu-id="c2464-117">Relationships</span></span>
<span data-ttu-id="c2464-118">Нет</span><span class="sxs-lookup"><span data-stu-id="c2464-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2464-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2464-119">JSON Representation</span></span>
<span data-ttu-id="c2464-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2464-120">Here is a JSON representation of the resource.</span></span>
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



