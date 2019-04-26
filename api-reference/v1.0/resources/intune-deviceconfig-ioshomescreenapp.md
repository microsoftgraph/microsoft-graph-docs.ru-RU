---
title: Тип ресурса iosHomeScreenApp
description: Представляет значок приложения на начальном экране
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67c11096414db0dccad2ccf56ec184a4e3f30397
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554739"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="65c6f-103">Тип ресурса iosHomeScreenApp</span><span class="sxs-lookup"><span data-stu-id="65c6f-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="65c6f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65c6f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65c6f-105">Представляет значок приложения на начальном экране</span><span class="sxs-lookup"><span data-stu-id="65c6f-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="65c6f-106">Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="65c6f-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65c6f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="65c6f-107">Properties</span></span>
|<span data-ttu-id="65c6f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="65c6f-108">Property</span></span>|<span data-ttu-id="65c6f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="65c6f-109">Type</span></span>|<span data-ttu-id="65c6f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="65c6f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65c6f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="65c6f-111">displayName</span></span>|<span data-ttu-id="65c6f-112">String</span><span class="sxs-lookup"><span data-stu-id="65c6f-112">String</span></span>|<span data-ttu-id="65c6f-113">Имя приложения. Наследуется от [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="65c6f-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="65c6f-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="65c6f-114">bundleID</span></span>|<span data-ttu-id="65c6f-115">String</span><span class="sxs-lookup"><span data-stu-id="65c6f-115">String</span></span>|<span data-ttu-id="65c6f-116">ИД пакета приложения</span><span class="sxs-lookup"><span data-stu-id="65c6f-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="65c6f-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="65c6f-117">Relationships</span></span>
<span data-ttu-id="65c6f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="65c6f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65c6f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65c6f-119">JSON Representation</span></span>
<span data-ttu-id="65c6f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65c6f-120">Here is a JSON representation of the resource.</span></span>
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



