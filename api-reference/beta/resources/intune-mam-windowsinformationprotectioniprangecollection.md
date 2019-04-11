---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3a972ddf469723acd91e6b122cfef103ab08e24f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785694"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="92fcb-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="92fcb-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="92fcb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="92fcb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92fcb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="92fcb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92fcb-106">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="92fcb-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="92fcb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="92fcb-107">Properties</span></span>
|<span data-ttu-id="92fcb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="92fcb-108">Property</span></span>|<span data-ttu-id="92fcb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="92fcb-109">Type</span></span>|<span data-ttu-id="92fcb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="92fcb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92fcb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="92fcb-111">displayName</span></span>|<span data-ttu-id="92fcb-112">String</span><span class="sxs-lookup"><span data-stu-id="92fcb-112">String</span></span>|<span data-ttu-id="92fcb-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="92fcb-113">Display name</span></span>|
|<span data-ttu-id="92fcb-114">ranges</span><span class="sxs-lookup"><span data-stu-id="92fcb-114">ranges</span></span>|<span data-ttu-id="92fcb-115">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="92fcb-115">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="92fcb-116">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="92fcb-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="92fcb-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="92fcb-117">Relationships</span></span>
<span data-ttu-id="92fcb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="92fcb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92fcb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="92fcb-119">JSON Representation</span></span>
<span data-ttu-id="92fcb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="92fcb-120">Here is a JSON representation of the resource.</span></span>
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





