---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 24c21b6260800250daa768df0684298f3bb142ae
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161826"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="08a62-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="08a62-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="08a62-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08a62-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08a62-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="08a62-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08a62-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="08a62-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08a62-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="08a62-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="08a62-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="08a62-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="08a62-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="08a62-109">Properties</span></span>
|<span data-ttu-id="08a62-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="08a62-110">Property</span></span>|<span data-ttu-id="08a62-111">Тип</span><span class="sxs-lookup"><span data-stu-id="08a62-111">Type</span></span>|<span data-ttu-id="08a62-112">Описание</span><span class="sxs-lookup"><span data-stu-id="08a62-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08a62-113">displayName</span><span class="sxs-lookup"><span data-stu-id="08a62-113">displayName</span></span>|<span data-ttu-id="08a62-114">String</span><span class="sxs-lookup"><span data-stu-id="08a62-114">String</span></span>|<span data-ttu-id="08a62-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="08a62-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="08a62-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="08a62-116">bundleID</span></span>|<span data-ttu-id="08a62-117">String</span><span class="sxs-lookup"><span data-stu-id="08a62-117">String</span></span>|<span data-ttu-id="08a62-118">BundleID приложения, если isWebClip имеет false или URL-адрес веб-клипа, если isWebClip имеет true.</span><span class="sxs-lookup"><span data-stu-id="08a62-118">BundleID of the app if isWebClip is false or the URL of a web clip if isWebClip is true.</span></span>|
|<span data-ttu-id="08a62-119">isWebClip</span><span class="sxs-lookup"><span data-stu-id="08a62-119">isWebClip</span></span>|<span data-ttu-id="08a62-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="08a62-120">Boolean</span></span>|<span data-ttu-id="08a62-121">Если задано true, то ИД пакета будет обрабатываться как URL-адрес для веб-клипа.</span><span class="sxs-lookup"><span data-stu-id="08a62-121">When true, the bundle ID will be handled as a URL for a web clip.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08a62-122">Связи</span><span class="sxs-lookup"><span data-stu-id="08a62-122">Relationships</span></span>
<span data-ttu-id="08a62-123">Нет</span><span class="sxs-lookup"><span data-stu-id="08a62-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08a62-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="08a62-124">JSON Representation</span></span>
<span data-ttu-id="08a62-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08a62-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String",
  "isWebClip": true
}
```




