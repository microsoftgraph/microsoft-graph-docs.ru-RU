---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c277bf90b14fec8408b918d1bbef99ad4ca21fa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780572"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="fe6a9-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="fe6a9-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="fe6a9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe6a9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe6a9-106">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="fe6a9-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="fe6a9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="fe6a9-107">Properties</span></span>
|<span data-ttu-id="fe6a9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="fe6a9-108">Property</span></span>|<span data-ttu-id="fe6a9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="fe6a9-109">Type</span></span>|<span data-ttu-id="fe6a9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fe6a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe6a9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="fe6a9-111">displayName</span></span>|<span data-ttu-id="fe6a9-112">String</span><span class="sxs-lookup"><span data-stu-id="fe6a9-112">String</span></span>|<span data-ttu-id="fe6a9-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="fe6a9-113">Display name</span></span>|
|<span data-ttu-id="fe6a9-114">ranges</span><span class="sxs-lookup"><span data-stu-id="fe6a9-114">ranges</span></span>|<span data-ttu-id="fe6a9-115">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="fe6a9-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="fe6a9-116">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="fe6a9-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe6a9-117">Связи</span><span class="sxs-lookup"><span data-stu-id="fe6a9-117">Relationships</span></span>
<span data-ttu-id="fe6a9-118">Нет</span><span class="sxs-lookup"><span data-stu-id="fe6a9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe6a9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fe6a9-119">JSON Representation</span></span>
<span data-ttu-id="fe6a9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fe6a9-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionIPRangeCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionIPRangeCollection",
  "displayName": "String",
  "ranges": [
    {
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```



