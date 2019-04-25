---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 026a69dc7697a0b779d72dfcab1695cf8c219d83
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550562"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="68eec-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="68eec-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="68eec-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="68eec-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68eec-105">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="68eec-105">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="68eec-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="68eec-106">Properties</span></span>
|<span data-ttu-id="68eec-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="68eec-107">Property</span></span>|<span data-ttu-id="68eec-108">Тип</span><span class="sxs-lookup"><span data-stu-id="68eec-108">Type</span></span>|<span data-ttu-id="68eec-109">Описание</span><span class="sxs-lookup"><span data-stu-id="68eec-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68eec-110">displayName</span><span class="sxs-lookup"><span data-stu-id="68eec-110">displayName</span></span>|<span data-ttu-id="68eec-111">String</span><span class="sxs-lookup"><span data-stu-id="68eec-111">String</span></span>|<span data-ttu-id="68eec-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="68eec-112">Display name</span></span>|
|<span data-ttu-id="68eec-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="68eec-113">proxiedDomains</span></span>|<span data-ttu-id="68eec-114">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="68eec-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="68eec-115">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="68eec-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="68eec-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="68eec-116">Relationships</span></span>
<span data-ttu-id="68eec-117">Нет</span><span class="sxs-lookup"><span data-stu-id="68eec-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68eec-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="68eec-118">JSON Representation</span></span>
<span data-ttu-id="68eec-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="68eec-119">Here is a JSON representation of the resource.</span></span>
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



