---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
ms.openlocfilehash: 63bcfe53cc2d3ee60b5f784e99798f1f97e883af
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334967"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="04f8c-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="04f8c-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="04f8c-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04f8c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04f8c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04f8c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04f8c-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="04f8c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04f8c-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="04f8c-107">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="04f8c-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="04f8c-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="04f8c-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="04f8c-109">Properties</span></span>
|<span data-ttu-id="04f8c-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="04f8c-110">Property</span></span>|<span data-ttu-id="04f8c-111">Тип</span><span class="sxs-lookup"><span data-stu-id="04f8c-111">Type</span></span>|<span data-ttu-id="04f8c-112">Описание</span><span class="sxs-lookup"><span data-stu-id="04f8c-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04f8c-113">displayName</span><span class="sxs-lookup"><span data-stu-id="04f8c-113">displayName</span></span>|<span data-ttu-id="04f8c-114">String</span><span class="sxs-lookup"><span data-stu-id="04f8c-114">String</span></span>|<span data-ttu-id="04f8c-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="04f8c-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="04f8c-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="04f8c-116">bundleID</span></span>|<span data-ttu-id="04f8c-117">String</span><span class="sxs-lookup"><span data-stu-id="04f8c-117">String</span></span>|<span data-ttu-id="04f8c-118">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="04f8c-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="04f8c-119">Связи</span><span class="sxs-lookup"><span data-stu-id="04f8c-119">Relationships</span></span>
<span data-ttu-id="04f8c-120">Нет</span><span class="sxs-lookup"><span data-stu-id="04f8c-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04f8c-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04f8c-121">JSON Representation</span></span>
<span data-ttu-id="04f8c-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04f8c-122">Here is a JSON representation of the resource.</span></span>
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





