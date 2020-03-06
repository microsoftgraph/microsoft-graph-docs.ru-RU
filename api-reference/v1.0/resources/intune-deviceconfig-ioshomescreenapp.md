---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c3cf96205d6484c61a6f4ec263566ccb9c2efaa
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532513"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="16f4d-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="16f4d-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="16f4d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="16f4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="16f4d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16f4d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16f4d-106">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="16f4d-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="16f4d-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="16f4d-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="16f4d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="16f4d-108">Properties</span></span>
|<span data-ttu-id="16f4d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="16f4d-109">Property</span></span>|<span data-ttu-id="16f4d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="16f4d-110">Type</span></span>|<span data-ttu-id="16f4d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="16f4d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16f4d-112">displayName</span><span class="sxs-lookup"><span data-stu-id="16f4d-112">displayName</span></span>|<span data-ttu-id="16f4d-113">Строка</span><span class="sxs-lookup"><span data-stu-id="16f4d-113">String</span></span>|<span data-ttu-id="16f4d-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="16f4d-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="16f4d-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="16f4d-115">bundleID</span></span>|<span data-ttu-id="16f4d-116">String</span><span class="sxs-lookup"><span data-stu-id="16f4d-116">String</span></span>|<span data-ttu-id="16f4d-117">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="16f4d-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="16f4d-118">Связи</span><span class="sxs-lookup"><span data-stu-id="16f4d-118">Relationships</span></span>
<span data-ttu-id="16f4d-119">Нет</span><span class="sxs-lookup"><span data-stu-id="16f4d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16f4d-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16f4d-120">JSON Representation</span></span>
<span data-ttu-id="16f4d-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16f4d-121">Here is a JSON representation of the resource.</span></span>
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




