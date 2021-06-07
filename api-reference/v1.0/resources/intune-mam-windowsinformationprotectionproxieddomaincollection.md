---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 987ae09f46c9bb2f0c6dc5481320d07ae250b01c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755730"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="65bfa-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="65bfa-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="65bfa-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65bfa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65bfa-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65bfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65bfa-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="65bfa-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="65bfa-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="65bfa-107">Properties</span></span>
|<span data-ttu-id="65bfa-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="65bfa-108">Property</span></span>|<span data-ttu-id="65bfa-109">Тип</span><span class="sxs-lookup"><span data-stu-id="65bfa-109">Type</span></span>|<span data-ttu-id="65bfa-110">Описание</span><span class="sxs-lookup"><span data-stu-id="65bfa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65bfa-111">displayName</span><span class="sxs-lookup"><span data-stu-id="65bfa-111">displayName</span></span>|<span data-ttu-id="65bfa-112">String</span><span class="sxs-lookup"><span data-stu-id="65bfa-112">String</span></span>|<span data-ttu-id="65bfa-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="65bfa-113">Display name</span></span>|
|<span data-ttu-id="65bfa-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="65bfa-114">proxiedDomains</span></span>|<span data-ttu-id="65bfa-115">Коллекция объектов [proxiedDomain](../resources/intune-mam-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="65bfa-115">[proxiedDomain](../resources/intune-mam-proxieddomain.md) collection</span></span>|<span data-ttu-id="65bfa-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="65bfa-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="65bfa-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="65bfa-117">Relationships</span></span>
<span data-ttu-id="65bfa-118">Нет</span><span class="sxs-lookup"><span data-stu-id="65bfa-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65bfa-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65bfa-119">JSON Representation</span></span>
<span data-ttu-id="65bfa-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65bfa-120">Here is a JSON representation of the resource.</span></span>
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




