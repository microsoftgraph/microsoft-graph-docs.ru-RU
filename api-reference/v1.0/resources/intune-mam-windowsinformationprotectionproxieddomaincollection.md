---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
ms.openlocfilehash: b19709bff695d9184cda5adbffd9e0591e46db2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027711"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="abf65-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="abf65-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="abf65-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="abf65-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="abf65-105">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="abf65-105">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="abf65-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="abf65-106">Properties</span></span>
|<span data-ttu-id="abf65-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="abf65-107">Property</span></span>|<span data-ttu-id="abf65-108">Тип</span><span class="sxs-lookup"><span data-stu-id="abf65-108">Type</span></span>|<span data-ttu-id="abf65-109">Описание</span><span class="sxs-lookup"><span data-stu-id="abf65-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="abf65-110">displayName</span><span class="sxs-lookup"><span data-stu-id="abf65-110">displayName</span></span>|<span data-ttu-id="abf65-111">Строка</span><span class="sxs-lookup"><span data-stu-id="abf65-111">String</span></span>|<span data-ttu-id="abf65-112">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="abf65-112">Display name</span></span>|
|<span data-ttu-id="abf65-113">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="abf65-113">proxiedDomains</span></span>|<span data-ttu-id="abf65-114">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="abf65-114">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="abf65-115">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="abf65-115">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="abf65-116">Связи</span><span class="sxs-lookup"><span data-stu-id="abf65-116">Relationships</span></span>
<span data-ttu-id="abf65-117">Нет</span><span class="sxs-lookup"><span data-stu-id="abf65-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="abf65-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="abf65-118">JSON Representation</span></span>
<span data-ttu-id="abf65-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="abf65-119">Here is a JSON representation of the resource.</span></span>
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



