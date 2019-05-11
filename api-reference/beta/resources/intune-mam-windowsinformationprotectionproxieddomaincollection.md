---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fc21b0f216c6daf3c8d12a9da80a18a05a6d3b8f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940542"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="6ec65-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="6ec65-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="6ec65-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6ec65-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ec65-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6ec65-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ec65-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="6ec65-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="6ec65-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ec65-107">Properties</span></span>
|<span data-ttu-id="6ec65-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ec65-108">Property</span></span>|<span data-ttu-id="6ec65-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6ec65-109">Type</span></span>|<span data-ttu-id="6ec65-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6ec65-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ec65-111">displayName</span><span class="sxs-lookup"><span data-stu-id="6ec65-111">displayName</span></span>|<span data-ttu-id="6ec65-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6ec65-112">String</span></span>|<span data-ttu-id="6ec65-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="6ec65-113">Display name</span></span>|
|<span data-ttu-id="6ec65-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="6ec65-114">proxiedDomains</span></span>|<span data-ttu-id="6ec65-115">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="6ec65-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="6ec65-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="6ec65-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ec65-117">Связи</span><span class="sxs-lookup"><span data-stu-id="6ec65-117">Relationships</span></span>
<span data-ttu-id="6ec65-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6ec65-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ec65-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ec65-119">JSON Representation</span></span>
<span data-ttu-id="6ec65-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ec65-120">Here is a JSON representation of the resource.</span></span>
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




