---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c25ca22acc8964c0578ad42e47088c108c7757c5
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360603"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="b1eed-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="b1eed-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="b1eed-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b1eed-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1eed-105">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="b1eed-105">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="b1eed-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="b1eed-106">Properties</span></span>
|<span data-ttu-id="b1eed-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="b1eed-107">Property</span></span>|<span data-ttu-id="b1eed-108">Тип</span><span class="sxs-lookup"><span data-stu-id="b1eed-108">Type</span></span>|<span data-ttu-id="b1eed-109">Описание</span><span class="sxs-lookup"><span data-stu-id="b1eed-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1eed-110">displayName</span><span class="sxs-lookup"><span data-stu-id="b1eed-110">displayName</span></span>|<span data-ttu-id="b1eed-111">String</span><span class="sxs-lookup"><span data-stu-id="b1eed-111">String</span></span>|<span data-ttu-id="b1eed-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="b1eed-112">Display name</span></span>|
|<span data-ttu-id="b1eed-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="b1eed-113">proxiedDomains</span></span>|<span data-ttu-id="b1eed-114">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="b1eed-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="b1eed-115">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="b1eed-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="b1eed-116">Связи</span><span class="sxs-lookup"><span data-stu-id="b1eed-116">Relationships</span></span>
<span data-ttu-id="b1eed-117">Нет</span><span class="sxs-lookup"><span data-stu-id="b1eed-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1eed-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b1eed-118">JSON Representation</span></span>
<span data-ttu-id="b1eed-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b1eed-119">Here is a JSON representation of the resource.</span></span>
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




