---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 06494127edffd919353b71d4541bbf5b4e019dcd
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49280496"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="b0fbd-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="b0fbd-103">iosHomeScreenApp resource type</span></span>

<span data-ttu-id="b0fbd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b0fbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b0fbd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0fbd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0fbd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0fbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0fbd-107">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="b0fbd-107">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="b0fbd-108">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b0fbd-108">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b0fbd-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0fbd-109">Properties</span></span>
|<span data-ttu-id="b0fbd-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0fbd-110">Property</span></span>|<span data-ttu-id="b0fbd-111">Тип</span><span class="sxs-lookup"><span data-stu-id="b0fbd-111">Type</span></span>|<span data-ttu-id="b0fbd-112">Описание</span><span class="sxs-lookup"><span data-stu-id="b0fbd-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0fbd-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b0fbd-113">displayName</span></span>|<span data-ttu-id="b0fbd-114">String</span><span class="sxs-lookup"><span data-stu-id="b0fbd-114">String</span></span>|<span data-ttu-id="b0fbd-115">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b0fbd-115">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="b0fbd-116">bundleID</span><span class="sxs-lookup"><span data-stu-id="b0fbd-116">bundleID</span></span>|<span data-ttu-id="b0fbd-117">String</span><span class="sxs-lookup"><span data-stu-id="b0fbd-117">String</span></span>|<span data-ttu-id="b0fbd-118">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="b0fbd-118">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0fbd-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b0fbd-119">Relationships</span></span>
<span data-ttu-id="b0fbd-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b0fbd-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0fbd-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0fbd-121">JSON Representation</span></span>
<span data-ttu-id="b0fbd-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0fbd-122">Here is a JSON representation of the resource.</span></span>
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




