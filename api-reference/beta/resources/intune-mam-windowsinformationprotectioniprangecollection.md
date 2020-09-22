---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 147961674ee9aa082b14e439ba6ead2cb4c618ae
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029991"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="b29f8-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="b29f8-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="b29f8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b29f8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b29f8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b29f8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b29f8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b29f8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b29f8-107">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="b29f8-107">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="b29f8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b29f8-108">Properties</span></span>
|<span data-ttu-id="b29f8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b29f8-109">Property</span></span>|<span data-ttu-id="b29f8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b29f8-110">Type</span></span>|<span data-ttu-id="b29f8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b29f8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b29f8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b29f8-112">displayName</span></span>|<span data-ttu-id="b29f8-113">String</span><span class="sxs-lookup"><span data-stu-id="b29f8-113">String</span></span>|<span data-ttu-id="b29f8-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="b29f8-114">Display name</span></span>|
|<span data-ttu-id="b29f8-115">ranges</span><span class="sxs-lookup"><span data-stu-id="b29f8-115">ranges</span></span>|<span data-ttu-id="b29f8-116">Коллекция объектов [ipRange](../resources/intune-shared-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="b29f8-116">[ipRange](../resources/intune-shared-iprange.md) collection</span></span>|<span data-ttu-id="b29f8-117">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="b29f8-117">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="b29f8-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="b29f8-118">Relationships</span></span>
<span data-ttu-id="b29f8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="b29f8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b29f8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b29f8-120">JSON Representation</span></span>
<span data-ttu-id="b29f8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b29f8-121">Here is a JSON representation of the resource.</span></span>
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
      "@odata.type": "microsoft.graph.ipRange"
    }
  ]
}
```






