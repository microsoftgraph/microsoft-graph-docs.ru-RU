---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 2cdaf6c263b041547056f8f6bd82e21ca880ebaa
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949179"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="e8bf3-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="e8bf3-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="e8bf3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e8bf3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8bf3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e8bf3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8bf3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e8bf3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8bf3-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="e8bf3-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="e8bf3-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8bf3-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e8bf3-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e8bf3-109">Properties</span></span>
|<span data-ttu-id="e8bf3-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e8bf3-110">Property</span></span>|<span data-ttu-id="e8bf3-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e8bf3-111">Type</span></span>|<span data-ttu-id="e8bf3-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e8bf3-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8bf3-113">displayName</span><span class="sxs-lookup"><span data-stu-id="e8bf3-113">displayName</span></span>|<span data-ttu-id="e8bf3-114">String</span><span class="sxs-lookup"><span data-stu-id="e8bf3-114">String</span></span>|<span data-ttu-id="e8bf3-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="e8bf3-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="e8bf3-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="e8bf3-116">bundleID</span></span>|<span data-ttu-id="e8bf3-117">String</span><span class="sxs-lookup"><span data-stu-id="e8bf3-117">String</span></span>|<span data-ttu-id="e8bf3-118">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="e8bf3-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="e8bf3-119">Связи</span><span class="sxs-lookup"><span data-stu-id="e8bf3-119">Relationships</span></span>
<span data-ttu-id="e8bf3-120">Нет</span><span class="sxs-lookup"><span data-stu-id="e8bf3-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e8bf3-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e8bf3-121">JSON Representation</span></span>
<span data-ttu-id="e8bf3-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e8bf3-122">Here is a JSON representation of the resource.</span></span>
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





