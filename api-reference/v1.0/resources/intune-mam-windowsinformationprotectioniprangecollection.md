---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a6a2f52613eae9d8e06751672c95230dfc3b00c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584826"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="16e7e-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="16e7e-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

> <span data-ttu-id="16e7e-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="16e7e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16e7e-105">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="16e7e-105">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="16e7e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="16e7e-106">Properties</span></span>
|<span data-ttu-id="16e7e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="16e7e-107">Property</span></span>|<span data-ttu-id="16e7e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="16e7e-108">Type</span></span>|<span data-ttu-id="16e7e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="16e7e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e7e-110">displayName</span><span class="sxs-lookup"><span data-stu-id="16e7e-110">displayName</span></span>|<span data-ttu-id="16e7e-111">String</span><span class="sxs-lookup"><span data-stu-id="16e7e-111">String</span></span>|<span data-ttu-id="16e7e-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="16e7e-112">Display name</span></span>|
|<span data-ttu-id="16e7e-113">ranges</span><span class="sxs-lookup"><span data-stu-id="16e7e-113">ranges</span></span>|<span data-ttu-id="16e7e-114">Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="16e7e-114">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="16e7e-115">Коллекция диапазонов адресов протокола Интернета</span><span class="sxs-lookup"><span data-stu-id="16e7e-115">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="16e7e-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="16e7e-116">Relationships</span></span>
<span data-ttu-id="16e7e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="16e7e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="16e7e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="16e7e-118">JSON Representation</span></span>
<span data-ttu-id="16e7e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="16e7e-119">Here is a JSON representation of the resource.</span></span>
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



