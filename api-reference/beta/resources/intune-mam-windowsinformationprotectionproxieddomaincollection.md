---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35c4f00965aa6878368e922a0c193484c90c6aed
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780362"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="671bb-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="671bb-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="671bb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="671bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="671bb-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="671bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="671bb-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="671bb-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="671bb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="671bb-107">Properties</span></span>
|<span data-ttu-id="671bb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="671bb-108">Property</span></span>|<span data-ttu-id="671bb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="671bb-109">Type</span></span>|<span data-ttu-id="671bb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="671bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="671bb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="671bb-111">displayName</span></span>|<span data-ttu-id="671bb-112">String</span><span class="sxs-lookup"><span data-stu-id="671bb-112">String</span></span>|<span data-ttu-id="671bb-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="671bb-113">Display name</span></span>|
|<span data-ttu-id="671bb-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="671bb-114">proxiedDomains</span></span>|<span data-ttu-id="671bb-115">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="671bb-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="671bb-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="671bb-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="671bb-117">Связи</span><span class="sxs-lookup"><span data-stu-id="671bb-117">Relationships</span></span>
<span data-ttu-id="671bb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="671bb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="671bb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="671bb-119">JSON Representation</span></span>
<span data-ttu-id="671bb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="671bb-120">Here is a JSON representation of the resource.</span></span>
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



