---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 11aa9af0dc075e7c07c61923722810e131bf2250
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448209"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="44838-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="44838-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="44838-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="44838-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="44838-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="44838-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44838-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="44838-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="44838-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="44838-107">Properties</span></span>
|<span data-ttu-id="44838-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="44838-108">Property</span></span>|<span data-ttu-id="44838-109">Тип</span><span class="sxs-lookup"><span data-stu-id="44838-109">Type</span></span>|<span data-ttu-id="44838-110">Описание</span><span class="sxs-lookup"><span data-stu-id="44838-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44838-111">displayName</span><span class="sxs-lookup"><span data-stu-id="44838-111">displayName</span></span>|<span data-ttu-id="44838-112">String</span><span class="sxs-lookup"><span data-stu-id="44838-112">String</span></span>|<span data-ttu-id="44838-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="44838-113">Display name</span></span>|
|<span data-ttu-id="44838-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="44838-114">proxiedDomains</span></span>|<span data-ttu-id="44838-115">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="44838-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="44838-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="44838-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="44838-117">Связи</span><span class="sxs-lookup"><span data-stu-id="44838-117">Relationships</span></span>
<span data-ttu-id="44838-118">Нет</span><span class="sxs-lookup"><span data-stu-id="44838-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="44838-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="44838-119">JSON Representation</span></span>
<span data-ttu-id="44838-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="44838-120">Here is a JSON representation of the resource.</span></span>
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




