---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 131694ba3ef67f1f87a1e40cd7545ad6e78717de
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43468399"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="00eb0-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="00eb0-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="00eb0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00eb0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="00eb0-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="00eb0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="00eb0-106">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="00eb0-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="00eb0-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="00eb0-107">Properties</span></span>
|<span data-ttu-id="00eb0-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="00eb0-108">Property</span></span>|<span data-ttu-id="00eb0-109">Тип</span><span class="sxs-lookup"><span data-stu-id="00eb0-109">Type</span></span>|<span data-ttu-id="00eb0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="00eb0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00eb0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="00eb0-111">displayName</span></span>|<span data-ttu-id="00eb0-112">String</span><span class="sxs-lookup"><span data-stu-id="00eb0-112">String</span></span>|<span data-ttu-id="00eb0-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="00eb0-113">Display name</span></span>|
|<span data-ttu-id="00eb0-114">ranges</span><span class="sxs-lookup"><span data-stu-id="00eb0-114">ranges</span></span>|<span data-ttu-id="00eb0-115">Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="00eb0-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="00eb0-116">Коллекция диапазонов адресов протокола Интернета</span><span class="sxs-lookup"><span data-stu-id="00eb0-116">Collection of Internet protocol address ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="00eb0-117">Связи</span><span class="sxs-lookup"><span data-stu-id="00eb0-117">Relationships</span></span>
<span data-ttu-id="00eb0-118">Нет</span><span class="sxs-lookup"><span data-stu-id="00eb0-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="00eb0-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="00eb0-119">JSON Representation</span></span>
<span data-ttu-id="00eb0-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="00eb0-120">Here is a JSON representation of the resource.</span></span>
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







