---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7f33614af89cc6bc7c5e69f56b9ebcface738362
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994414"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="d2feb-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="d2feb-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="d2feb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d2feb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2feb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d2feb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2feb-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="d2feb-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="d2feb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d2feb-107">Properties</span></span>
|<span data-ttu-id="d2feb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d2feb-108">Property</span></span>|<span data-ttu-id="d2feb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d2feb-109">Type</span></span>|<span data-ttu-id="d2feb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d2feb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2feb-111">displayName</span><span class="sxs-lookup"><span data-stu-id="d2feb-111">displayName</span></span>|<span data-ttu-id="d2feb-112">String</span><span class="sxs-lookup"><span data-stu-id="d2feb-112">String</span></span>|<span data-ttu-id="d2feb-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="d2feb-113">Display name</span></span>|
|<span data-ttu-id="d2feb-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="d2feb-114">proxiedDomains</span></span>|<span data-ttu-id="d2feb-115">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="d2feb-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="d2feb-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="d2feb-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2feb-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="d2feb-117">Relationships</span></span>
<span data-ttu-id="d2feb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d2feb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2feb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d2feb-119">JSON Representation</span></span>
<span data-ttu-id="d2feb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d2feb-120">Here is a JSON representation of the resource.</span></span>
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





