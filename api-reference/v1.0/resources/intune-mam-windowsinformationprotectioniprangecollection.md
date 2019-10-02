---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1774a52b6dd5535443bb24dea5e786fc2c8cff34
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360645"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="51e82-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="51e82-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="51e82-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51e82-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51e82-105">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="51e82-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="51e82-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="51e82-106">Properties</span></span>
|<span data-ttu-id="51e82-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="51e82-107">Property</span></span>|<span data-ttu-id="51e82-108">Тип</span><span class="sxs-lookup"><span data-stu-id="51e82-108">Type</span></span>|<span data-ttu-id="51e82-109">Описание</span><span class="sxs-lookup"><span data-stu-id="51e82-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e82-110">displayName</span><span class="sxs-lookup"><span data-stu-id="51e82-110">displayName</span></span>|<span data-ttu-id="51e82-111">String</span><span class="sxs-lookup"><span data-stu-id="51e82-111">String</span></span>|<span data-ttu-id="51e82-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="51e82-112">Display name</span></span>|
|<span data-ttu-id="51e82-113">ranges</span><span class="sxs-lookup"><span data-stu-id="51e82-113">ranges</span></span>|<span data-ttu-id="51e82-114">Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="51e82-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="51e82-115">Коллекция диапазонов адресов протокола Интернета</span><span class="sxs-lookup"><span data-stu-id="51e82-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="51e82-116">Связи</span><span class="sxs-lookup"><span data-stu-id="51e82-116">Relationships</span></span>
<span data-ttu-id="51e82-117">Нет</span><span class="sxs-lookup"><span data-stu-id="51e82-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51e82-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51e82-118">JSON Representation</span></span>
<span data-ttu-id="51e82-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51e82-119">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange",
      "lowerAddress": "String",
      "upperAddress": "String"
    }
  ]
}
```




