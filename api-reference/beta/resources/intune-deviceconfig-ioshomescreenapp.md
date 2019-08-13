---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1a491f6dc8dbbdce729bfebb732f94222ef2b03e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357035"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="b23ca-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="b23ca-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="b23ca-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b23ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b23ca-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b23ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b23ca-106">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="b23ca-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="b23ca-107">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b23ca-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b23ca-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b23ca-108">Properties</span></span>
|<span data-ttu-id="b23ca-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b23ca-109">Property</span></span>|<span data-ttu-id="b23ca-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b23ca-110">Type</span></span>|<span data-ttu-id="b23ca-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b23ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b23ca-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b23ca-112">displayName</span></span>|<span data-ttu-id="b23ca-113">String</span><span class="sxs-lookup"><span data-stu-id="b23ca-113">String</span></span>|<span data-ttu-id="b23ca-114">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="b23ca-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="b23ca-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="b23ca-115">bundleID</span></span>|<span data-ttu-id="b23ca-116">String</span><span class="sxs-lookup"><span data-stu-id="b23ca-116">String</span></span>|<span data-ttu-id="b23ca-117">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="b23ca-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="b23ca-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b23ca-118">Relationships</span></span>
<span data-ttu-id="b23ca-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b23ca-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b23ca-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b23ca-120">JSON Representation</span></span>
<span data-ttu-id="b23ca-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b23ca-121">Here is a JSON representation of the resource.</span></span>
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



