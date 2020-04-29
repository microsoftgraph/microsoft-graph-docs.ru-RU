---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ed97494144d6e8bb7e4154a84d0b4f2e7c01cf3
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43410717"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="52c3f-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="52c3f-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="52c3f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52c3f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="52c3f-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="52c3f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52c3f-106">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="52c3f-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="52c3f-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="52c3f-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="52c3f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="52c3f-108">Properties</span></span>
|<span data-ttu-id="52c3f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="52c3f-109">Property</span></span>|<span data-ttu-id="52c3f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="52c3f-110">Type</span></span>|<span data-ttu-id="52c3f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="52c3f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52c3f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="52c3f-112">displayName</span></span>|<span data-ttu-id="52c3f-113">String</span><span class="sxs-lookup"><span data-stu-id="52c3f-113">String</span></span>|<span data-ttu-id="52c3f-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="52c3f-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="52c3f-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="52c3f-115">bundleID</span></span>|<span data-ttu-id="52c3f-116">String</span><span class="sxs-lookup"><span data-stu-id="52c3f-116">String</span></span>|<span data-ttu-id="52c3f-117">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="52c3f-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="52c3f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="52c3f-118">Relationships</span></span>
<span data-ttu-id="52c3f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="52c3f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52c3f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52c3f-120">JSON Representation</span></span>
<span data-ttu-id="52c3f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52c3f-121">Here is a JSON representation of the resource.</span></span>
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







