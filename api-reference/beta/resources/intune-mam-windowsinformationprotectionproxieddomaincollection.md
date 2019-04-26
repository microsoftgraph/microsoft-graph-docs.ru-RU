---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0cf20d0a0afb33732278b9c8f988b3008854b770
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558295"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="f48e1-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="f48e1-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="f48e1-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f48e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f48e1-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f48e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f48e1-106">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="f48e1-106">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="f48e1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f48e1-107">Properties</span></span>
|<span data-ttu-id="f48e1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f48e1-108">Property</span></span>|<span data-ttu-id="f48e1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f48e1-109">Type</span></span>|<span data-ttu-id="f48e1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f48e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f48e1-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f48e1-111">displayName</span></span>|<span data-ttu-id="f48e1-112">String</span><span class="sxs-lookup"><span data-stu-id="f48e1-112">String</span></span>|<span data-ttu-id="f48e1-113">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="f48e1-113">Display name</span></span>|
|<span data-ttu-id="f48e1-114">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="f48e1-114">proxiedDomains</span></span>|<span data-ttu-id="f48e1-115">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="f48e1-115">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="f48e1-116">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="f48e1-116">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="f48e1-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="f48e1-117">Relationships</span></span>
<span data-ttu-id="f48e1-118">Нет</span><span class="sxs-lookup"><span data-stu-id="f48e1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f48e1-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f48e1-119">JSON Representation</span></span>
<span data-ttu-id="f48e1-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f48e1-120">Here is a JSON representation of the resource.</span></span>
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





