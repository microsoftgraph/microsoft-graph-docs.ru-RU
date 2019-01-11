---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 39db8de19fbfc568f85c4930e8c3124ffea2dd57
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850598"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="796a1-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="796a1-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="796a1-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="796a1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="796a1-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="796a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="796a1-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="796a1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="796a1-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="796a1-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="796a1-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="796a1-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="796a1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="796a1-109">Properties</span></span>
|<span data-ttu-id="796a1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="796a1-110">Property</span></span>|<span data-ttu-id="796a1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="796a1-111">Type</span></span>|<span data-ttu-id="796a1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="796a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="796a1-113">displayName</span><span class="sxs-lookup"><span data-stu-id="796a1-113">displayName</span></span>|<span data-ttu-id="796a1-114">String</span><span class="sxs-lookup"><span data-stu-id="796a1-114">String</span></span>|<span data-ttu-id="796a1-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="796a1-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="796a1-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="796a1-116">bundleID</span></span>|<span data-ttu-id="796a1-117">String</span><span class="sxs-lookup"><span data-stu-id="796a1-117">String</span></span>|<span data-ttu-id="796a1-118">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="796a1-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="796a1-119">Связи</span><span class="sxs-lookup"><span data-stu-id="796a1-119">Relationships</span></span>
<span data-ttu-id="796a1-120">Нет</span><span class="sxs-lookup"><span data-stu-id="796a1-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="796a1-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="796a1-121">JSON Representation</span></span>
<span data-ttu-id="796a1-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="796a1-122">Here is a JSON representation of the resource.</span></span>
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





