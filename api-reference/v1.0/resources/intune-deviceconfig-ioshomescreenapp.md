---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bb63950229f88fb9987e75f42abfbe39793864ad
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845698"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="44bfc-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="44bfc-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="44bfc-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="44bfc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="44bfc-105">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="44bfc-105">Represents an icon for an app on the Home Screen</span></span>

<span data-ttu-id="44bfc-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="44bfc-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="44bfc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="44bfc-107">Properties</span></span>
|<span data-ttu-id="44bfc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="44bfc-108">Property</span></span>|<span data-ttu-id="44bfc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="44bfc-109">Type</span></span>|<span data-ttu-id="44bfc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="44bfc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44bfc-111">displayName</span><span class="sxs-lookup"><span data-stu-id="44bfc-111">displayName</span></span>|<span data-ttu-id="44bfc-112">String</span><span class="sxs-lookup"><span data-stu-id="44bfc-112">String</span></span>|<span data-ttu-id="44bfc-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="44bfc-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="44bfc-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="44bfc-114">bundleID</span></span>|<span data-ttu-id="44bfc-115">String</span><span class="sxs-lookup"><span data-stu-id="44bfc-115">String</span></span>|<span data-ttu-id="44bfc-116">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="44bfc-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="44bfc-117">Связи</span><span class="sxs-lookup"><span data-stu-id="44bfc-117">Relationships</span></span>
<span data-ttu-id="44bfc-118">Нет</span><span class="sxs-lookup"><span data-stu-id="44bfc-118">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="44bfc-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44bfc-119">JSON Representation</span></span>
<span data-ttu-id="44bfc-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44bfc-120">Here is a JSON representation of the resource.</span></span>
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



