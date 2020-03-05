---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fb77a9a359ebd06b788470cf5948c6f4b92780c4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448230"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="cce75-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="cce75-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="cce75-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="cce75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cce75-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cce75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cce75-106">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="cce75-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="cce75-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="cce75-107">Properties</span></span>
|<span data-ttu-id="cce75-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="cce75-108">Property</span></span>|<span data-ttu-id="cce75-109">Тип</span><span class="sxs-lookup"><span data-stu-id="cce75-109">Type</span></span>|<span data-ttu-id="cce75-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cce75-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cce75-111">displayName</span><span class="sxs-lookup"><span data-stu-id="cce75-111">displayName</span></span>|<span data-ttu-id="cce75-112">String</span><span class="sxs-lookup"><span data-stu-id="cce75-112">String</span></span>|<span data-ttu-id="cce75-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="cce75-113">Display name</span></span>|
|<span data-ttu-id="cce75-114">ranges</span><span class="sxs-lookup"><span data-stu-id="cce75-114">ranges</span></span>|<span data-ttu-id="cce75-115">Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="cce75-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="cce75-116">Коллекция диапазонов адресов протокола Интернета</span><span class="sxs-lookup"><span data-stu-id="cce75-116">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="cce75-117">Связи</span><span class="sxs-lookup"><span data-stu-id="cce75-117">Relationships</span></span>
<span data-ttu-id="cce75-118">Нет</span><span class="sxs-lookup"><span data-stu-id="cce75-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cce75-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cce75-119">JSON Representation</span></span>
<span data-ttu-id="cce75-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cce75-120">Here is a JSON representation of the resource.</span></span>
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




