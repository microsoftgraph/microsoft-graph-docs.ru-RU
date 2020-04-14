---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a00cfc03ff6b98bb32b7c8fe7e9d747f15040d68
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419294"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="91854-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="91854-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

<span data-ttu-id="91854-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91854-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91854-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91854-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91854-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91854-107">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="91854-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="91854-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="91854-108">Properties</span></span>
|<span data-ttu-id="91854-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="91854-109">Property</span></span>|<span data-ttu-id="91854-110">Тип</span><span class="sxs-lookup"><span data-stu-id="91854-110">Type</span></span>|<span data-ttu-id="91854-111">Описание</span><span class="sxs-lookup"><span data-stu-id="91854-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91854-112">displayName</span><span class="sxs-lookup"><span data-stu-id="91854-112">displayName</span></span>|<span data-ttu-id="91854-113">String</span><span class="sxs-lookup"><span data-stu-id="91854-113">String</span></span>|<span data-ttu-id="91854-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="91854-114">Display name</span></span>|
|<span data-ttu-id="91854-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="91854-115">proxiedDomains</span></span>|<span data-ttu-id="91854-116">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="91854-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="91854-117">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="91854-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="91854-118">Связи</span><span class="sxs-lookup"><span data-stu-id="91854-118">Relationships</span></span>
<span data-ttu-id="91854-119">Нет</span><span class="sxs-lookup"><span data-stu-id="91854-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91854-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91854-120">JSON Representation</span></span>
<span data-ttu-id="91854-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91854-121">Here is a JSON representation of the resource.</span></span>
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



