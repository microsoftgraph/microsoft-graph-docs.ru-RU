---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: dfc07b47115e4e5ce4be959ac7867a2963021abf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822101"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="a1ac2-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="a1ac2-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="a1ac2-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1ac2-105">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="a1ac2-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="a1ac2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a1ac2-106">Properties</span></span>
|<span data-ttu-id="a1ac2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a1ac2-107">Property</span></span>|<span data-ttu-id="a1ac2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a1ac2-108">Type</span></span>|<span data-ttu-id="a1ac2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a1ac2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1ac2-110">displayName</span><span class="sxs-lookup"><span data-stu-id="a1ac2-110">displayName</span></span>|<span data-ttu-id="a1ac2-111">Строка</span><span class="sxs-lookup"><span data-stu-id="a1ac2-111">String</span></span>|<span data-ttu-id="a1ac2-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="a1ac2-112">Display name</span></span>|
|<span data-ttu-id="a1ac2-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="a1ac2-113">proxiedDomains</span></span>|<span data-ttu-id="a1ac2-114">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="a1ac2-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="a1ac2-115">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="a1ac2-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="a1ac2-116">Связи</span><span class="sxs-lookup"><span data-stu-id="a1ac2-116">Relationships</span></span>
<span data-ttu-id="a1ac2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="a1ac2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a1ac2-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a1ac2-118">JSON Representation</span></span>
<span data-ttu-id="a1ac2-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a1ac2-119">Here is a JSON representation of the resource.</span></span>
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



