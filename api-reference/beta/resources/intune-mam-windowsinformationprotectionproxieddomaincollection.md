---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 044a257810cc3039f2022d948632207f2bb06262
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029927"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="695e8-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="695e8-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="695e8-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="695e8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="695e8-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="695e8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="695e8-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="695e8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="695e8-107">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="695e8-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="695e8-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="695e8-108">Properties</span></span>
|<span data-ttu-id="695e8-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="695e8-109">Property</span></span>|<span data-ttu-id="695e8-110">Тип</span><span class="sxs-lookup"><span data-stu-id="695e8-110">Type</span></span>|<span data-ttu-id="695e8-111">Описание</span><span class="sxs-lookup"><span data-stu-id="695e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="695e8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="695e8-112">displayName</span></span>|<span data-ttu-id="695e8-113">String</span><span class="sxs-lookup"><span data-stu-id="695e8-113">String</span></span>|<span data-ttu-id="695e8-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="695e8-114">Display name</span></span>|
|<span data-ttu-id="695e8-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="695e8-115">proxiedDomains</span></span>|<span data-ttu-id="695e8-116">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="695e8-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="695e8-117">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="695e8-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="695e8-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="695e8-118">Relationships</span></span>
<span data-ttu-id="695e8-119">Нет</span><span class="sxs-lookup"><span data-stu-id="695e8-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="695e8-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="695e8-120">JSON Representation</span></span>
<span data-ttu-id="695e8-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="695e8-121">Here is a JSON representation of the resource.</span></span>
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






