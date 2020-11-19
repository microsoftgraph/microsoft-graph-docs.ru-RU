---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 32b05c1c2a9d830a0951f981d0e5b1594e5ae486
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207227"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="76e4f-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="76e4f-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="76e4f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76e4f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76e4f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="76e4f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76e4f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="76e4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76e4f-107">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="76e4f-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="76e4f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="76e4f-108">Properties</span></span>
|<span data-ttu-id="76e4f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="76e4f-109">Property</span></span>|<span data-ttu-id="76e4f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="76e4f-110">Type</span></span>|<span data-ttu-id="76e4f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="76e4f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76e4f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="76e4f-112">displayName</span></span>|<span data-ttu-id="76e4f-113">String</span><span class="sxs-lookup"><span data-stu-id="76e4f-113">String</span></span>|<span data-ttu-id="76e4f-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="76e4f-114">Display name</span></span>|
|<span data-ttu-id="76e4f-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="76e4f-115">proxiedDomains</span></span>|<span data-ttu-id="76e4f-116">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="76e4f-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="76e4f-117">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="76e4f-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="76e4f-118">Связи</span><span class="sxs-lookup"><span data-stu-id="76e4f-118">Relationships</span></span>
<span data-ttu-id="76e4f-119">Нет</span><span class="sxs-lookup"><span data-stu-id="76e4f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="76e4f-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="76e4f-120">JSON Representation</span></span>
<span data-ttu-id="76e4f-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="76e4f-121">Here is a JSON representation of the resource.</span></span>
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




