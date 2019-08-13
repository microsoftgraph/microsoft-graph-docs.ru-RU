---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cccaf79205dfd0114a3d26dae1fd547d07811d42
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342105"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="af272-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="af272-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="af272-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="af272-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af272-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="af272-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af272-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="af272-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="af272-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="af272-107">Properties</span></span>
|<span data-ttu-id="af272-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="af272-108">Property</span></span>|<span data-ttu-id="af272-109">Тип</span><span class="sxs-lookup"><span data-stu-id="af272-109">Type</span></span>|<span data-ttu-id="af272-110">Описание</span><span class="sxs-lookup"><span data-stu-id="af272-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af272-111">displayName</span><span class="sxs-lookup"><span data-stu-id="af272-111">displayName</span></span>|<span data-ttu-id="af272-112">String</span><span class="sxs-lookup"><span data-stu-id="af272-112">String</span></span>|<span data-ttu-id="af272-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="af272-113">Display name</span></span>|
|<span data-ttu-id="af272-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="af272-114">proxiedDomains</span></span>|<span data-ttu-id="af272-115">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="af272-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="af272-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="af272-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="af272-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="af272-117">Relationships</span></span>
<span data-ttu-id="af272-118">Нет</span><span class="sxs-lookup"><span data-stu-id="af272-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="af272-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="af272-119">JSON Representation</span></span>
<span data-ttu-id="af272-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="af272-120">Here is a JSON representation of the resource.</span></span>
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



