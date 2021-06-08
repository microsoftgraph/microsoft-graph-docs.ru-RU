---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: de16278256e9c6860a3cdead2ab5e940d0878a1a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760080"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="16c9d-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="16c9d-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="16c9d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16c9d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16c9d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16c9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16c9d-106">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="16c9d-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="16c9d-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="16c9d-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16c9d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="16c9d-108">Properties</span></span>
|<span data-ttu-id="16c9d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="16c9d-109">Property</span></span>|<span data-ttu-id="16c9d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="16c9d-110">Type</span></span>|<span data-ttu-id="16c9d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="16c9d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16c9d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="16c9d-112">displayName</span></span>|<span data-ttu-id="16c9d-113">String</span><span class="sxs-lookup"><span data-stu-id="16c9d-113">String</span></span>|<span data-ttu-id="16c9d-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="16c9d-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="16c9d-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="16c9d-115">bundleID</span></span>|<span data-ttu-id="16c9d-116">String</span><span class="sxs-lookup"><span data-stu-id="16c9d-116">String</span></span>|<span data-ttu-id="16c9d-117">BundleID приложения, если isWebClip является ложным или URL-адрес веб-клипа, если isWebClip является правдой.</span><span class="sxs-lookup"><span data-stu-id="16c9d-117">BundleID of the app if isWebClip is false or the URL of a web clip if isWebClip is true.</span></span>|

## <a name="relationships"></a><span data-ttu-id="16c9d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="16c9d-118">Relationships</span></span>
<span data-ttu-id="16c9d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="16c9d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16c9d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16c9d-120">JSON Representation</span></span>
<span data-ttu-id="16c9d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16c9d-121">Here is a JSON representation of the resource.</span></span>
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




