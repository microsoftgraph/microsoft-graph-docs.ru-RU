---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
ms.openlocfilehash: 5c8700e0164bebbe6e930ebbd07a01c27c0f2495
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075711"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="91235-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="91235-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="91235-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="91235-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="91235-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91235-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="91235-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="91235-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="91235-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="91235-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="91235-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="91235-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="91235-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="91235-109">Properties</span></span>
|<span data-ttu-id="91235-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="91235-110">Property</span></span>|<span data-ttu-id="91235-111">Тип</span><span class="sxs-lookup"><span data-stu-id="91235-111">Type</span></span>|<span data-ttu-id="91235-112">Описание</span><span class="sxs-lookup"><span data-stu-id="91235-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91235-113">displayName</span><span class="sxs-lookup"><span data-stu-id="91235-113">displayName</span></span>|<span data-ttu-id="91235-114">String</span><span class="sxs-lookup"><span data-stu-id="91235-114">String</span></span>|<span data-ttu-id="91235-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="91235-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="91235-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="91235-116">bundleID</span></span>|<span data-ttu-id="91235-117">String</span><span class="sxs-lookup"><span data-stu-id="91235-117">String</span></span>|<span data-ttu-id="91235-118">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="91235-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="91235-119">Связи</span><span class="sxs-lookup"><span data-stu-id="91235-119">Relationships</span></span>
<span data-ttu-id="91235-120">Нет</span><span class="sxs-lookup"><span data-stu-id="91235-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="91235-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91235-121">JSON Representation</span></span>
<span data-ttu-id="91235-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91235-122">Here is a JSON representation of the resource.</span></span>
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





