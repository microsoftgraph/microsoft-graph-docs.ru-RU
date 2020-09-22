---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8df7439bec871e8b4c7ea1a8f15829b60f2fa21f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48086534"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="1f3d9-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="1f3d9-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="1f3d9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1f3d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1f3d9-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1f3d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1f3d9-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="1f3d9-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="1f3d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1f3d9-107">Properties</span></span>
|<span data-ttu-id="1f3d9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1f3d9-108">Property</span></span>|<span data-ttu-id="1f3d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1f3d9-109">Type</span></span>|<span data-ttu-id="1f3d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1f3d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f3d9-111">displayName</span><span class="sxs-lookup"><span data-stu-id="1f3d9-111">displayName</span></span>|<span data-ttu-id="1f3d9-112">Строка</span><span class="sxs-lookup"><span data-stu-id="1f3d9-112">String</span></span>|<span data-ttu-id="1f3d9-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="1f3d9-113">Display name</span></span>|
|<span data-ttu-id="1f3d9-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="1f3d9-114">proxiedDomains</span></span>|<span data-ttu-id="1f3d9-115">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="1f3d9-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="1f3d9-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="1f3d9-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f3d9-117">Связи</span><span class="sxs-lookup"><span data-stu-id="1f3d9-117">Relationships</span></span>
<span data-ttu-id="1f3d9-118">Нет</span><span class="sxs-lookup"><span data-stu-id="1f3d9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1f3d9-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1f3d9-119">JSON Representation</span></span>
<span data-ttu-id="1f3d9-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1f3d9-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionProxiedDomainCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionProxiedDomainCollection",
  "displayName": "String",
  "proxiedDomains": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ]
}
```









