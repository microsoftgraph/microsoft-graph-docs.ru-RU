---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: tfitzmac
ms.openlocfilehash: 3a385710dc38b5fb5927ee55e558fef67341585f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339349"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="872f9-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="872f9-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="872f9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="872f9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="872f9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="872f9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="872f9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="872f9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="872f9-107">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="872f9-107">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="872f9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="872f9-108">Properties</span></span>
|<span data-ttu-id="872f9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="872f9-109">Property</span></span>|<span data-ttu-id="872f9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="872f9-110">Type</span></span>|<span data-ttu-id="872f9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="872f9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="872f9-112">displayName</span><span class="sxs-lookup"><span data-stu-id="872f9-112">displayName</span></span>|<span data-ttu-id="872f9-113">Строка</span><span class="sxs-lookup"><span data-stu-id="872f9-113">String</span></span>|<span data-ttu-id="872f9-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="872f9-114">Display name</span></span>|
|<span data-ttu-id="872f9-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="872f9-115">proxiedDomains</span></span>|<span data-ttu-id="872f9-116">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="872f9-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="872f9-117">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="872f9-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="872f9-118">Связи</span><span class="sxs-lookup"><span data-stu-id="872f9-118">Relationships</span></span>
<span data-ttu-id="872f9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="872f9-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="872f9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="872f9-120">JSON Representation</span></span>
<span data-ttu-id="872f9-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="872f9-121">Here is a JSON representation of the resource.</span></span>
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





