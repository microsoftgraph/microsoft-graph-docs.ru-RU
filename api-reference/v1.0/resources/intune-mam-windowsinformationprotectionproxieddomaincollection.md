---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 500f662b0a610866ac3e637850f5fd6edeffaa5b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459695"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="51482-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="51482-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="51482-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51482-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51482-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="51482-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51482-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="51482-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="51482-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="51482-107">Properties</span></span>
|<span data-ttu-id="51482-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="51482-108">Property</span></span>|<span data-ttu-id="51482-109">Тип</span><span class="sxs-lookup"><span data-stu-id="51482-109">Type</span></span>|<span data-ttu-id="51482-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51482-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51482-111">displayName</span><span class="sxs-lookup"><span data-stu-id="51482-111">displayName</span></span>|<span data-ttu-id="51482-112">String</span><span class="sxs-lookup"><span data-stu-id="51482-112">String</span></span>|<span data-ttu-id="51482-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="51482-113">Display name</span></span>|
|<span data-ttu-id="51482-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="51482-114">proxiedDomains</span></span>|<span data-ttu-id="51482-115">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="51482-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="51482-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="51482-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="51482-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="51482-117">Relationships</span></span>
<span data-ttu-id="51482-118">Нет</span><span class="sxs-lookup"><span data-stu-id="51482-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51482-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="51482-119">JSON Representation</span></span>
<span data-ttu-id="51482-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="51482-120">Here is a JSON representation of the resource.</span></span>
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







