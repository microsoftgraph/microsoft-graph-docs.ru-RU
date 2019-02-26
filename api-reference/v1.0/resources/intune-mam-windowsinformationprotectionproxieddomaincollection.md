---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 026a69dc7697a0b779d72dfcab1695cf8c219d83
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264332"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="22deb-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="22deb-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="22deb-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="22deb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22deb-105">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="22deb-105">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="22deb-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="22deb-106">Properties</span></span>
|<span data-ttu-id="22deb-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="22deb-107">Property</span></span>|<span data-ttu-id="22deb-108">Тип</span><span class="sxs-lookup"><span data-stu-id="22deb-108">Type</span></span>|<span data-ttu-id="22deb-109">Описание</span><span class="sxs-lookup"><span data-stu-id="22deb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22deb-110">displayName</span><span class="sxs-lookup"><span data-stu-id="22deb-110">displayName</span></span>|<span data-ttu-id="22deb-111">Строка</span><span class="sxs-lookup"><span data-stu-id="22deb-111">String</span></span>|<span data-ttu-id="22deb-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="22deb-112">Display name</span></span>|
|<span data-ttu-id="22deb-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="22deb-113">proxiedDomains</span></span>|<span data-ttu-id="22deb-114">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="22deb-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="22deb-115">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="22deb-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="22deb-116">Связи</span><span class="sxs-lookup"><span data-stu-id="22deb-116">Relationships</span></span>
<span data-ttu-id="22deb-117">Нет</span><span class="sxs-lookup"><span data-stu-id="22deb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="22deb-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22deb-118">JSON Representation</span></span>
<span data-ttu-id="22deb-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22deb-119">Here is a JSON representation of the resource.</span></span>
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



