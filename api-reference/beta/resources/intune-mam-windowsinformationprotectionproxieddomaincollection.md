---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: df71cd36a84a0b0782b645cf56df708d1f30e365
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855127"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="c30b3-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="c30b3-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="c30b3-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c30b3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c30b3-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c30b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c30b3-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c30b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c30b3-107">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="c30b3-107">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="c30b3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c30b3-108">Properties</span></span>
|<span data-ttu-id="c30b3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c30b3-109">Property</span></span>|<span data-ttu-id="c30b3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c30b3-110">Type</span></span>|<span data-ttu-id="c30b3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c30b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c30b3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c30b3-112">displayName</span></span>|<span data-ttu-id="c30b3-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c30b3-113">String</span></span>|<span data-ttu-id="c30b3-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="c30b3-114">Display name</span></span>|
|<span data-ttu-id="c30b3-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="c30b3-115">proxiedDomains</span></span>|<span data-ttu-id="c30b3-116">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="c30b3-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="c30b3-117">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="c30b3-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="c30b3-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c30b3-118">Relationships</span></span>
<span data-ttu-id="c30b3-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c30b3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c30b3-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c30b3-120">JSON Representation</span></span>
<span data-ttu-id="c30b3-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c30b3-121">Here is a JSON representation of the resource.</span></span>
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





