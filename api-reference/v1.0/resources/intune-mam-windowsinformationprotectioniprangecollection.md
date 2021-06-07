---
title: Тип ресурса windowsInformationProtectionIPRangeCollection
description: Коллекция диапазонов IP-адресов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 722e96e69027cccb666bc789fc7516b914b975bb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752310"
---
# <a name="windowsinformationprotectioniprangecollection-resource-type"></a><span data-ttu-id="6f5cb-103">Тип ресурса windowsInformationProtectionIPRangeCollection</span><span class="sxs-lookup"><span data-stu-id="6f5cb-103">windowsInformationProtectionIPRangeCollection resource type</span></span>

<span data-ttu-id="6f5cb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f5cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f5cb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6f5cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f5cb-106">Коллекция диапазонов IP-адресов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="6f5cb-106">Windows Information Protection IP Range Collection</span></span>

## <a name="properties"></a><span data-ttu-id="6f5cb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6f5cb-107">Properties</span></span>
|<span data-ttu-id="6f5cb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6f5cb-108">Property</span></span>|<span data-ttu-id="6f5cb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6f5cb-109">Type</span></span>|<span data-ttu-id="6f5cb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6f5cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f5cb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6f5cb-111">displayName</span></span>|<span data-ttu-id="6f5cb-112">String</span><span class="sxs-lookup"><span data-stu-id="6f5cb-112">String</span></span>|<span data-ttu-id="6f5cb-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="6f5cb-113">Display name</span></span>|
|<span data-ttu-id="6f5cb-114">ranges</span><span class="sxs-lookup"><span data-stu-id="6f5cb-114">ranges</span></span>|<span data-ttu-id="6f5cb-115">Коллекция объектов [ipRange](../resources/intune-mam-iprange.md)</span><span class="sxs-lookup"><span data-stu-id="6f5cb-115">[ipRange](../resources/intune-mam-iprange.md) collection</span></span>|<span data-ttu-id="6f5cb-116">Коллекция диапазонов IP-адресов</span><span class="sxs-lookup"><span data-stu-id="6f5cb-116">Collection of ip ranges</span></span>|

## <a name="relationships"></a><span data-ttu-id="6f5cb-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="6f5cb-117">Relationships</span></span>
<span data-ttu-id="6f5cb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6f5cb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6f5cb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6f5cb-119">JSON Representation</span></span>
<span data-ttu-id="6f5cb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6f5cb-120">Here is a JSON representation of the resource.</span></span>
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




