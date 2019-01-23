---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c65a4b6a94f317c5d75b440aeef7fe387496be32
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421678"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="db845-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="db845-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="db845-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="db845-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="db845-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="db845-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="db845-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="db845-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="db845-107">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="db845-107">Windows Information Protection Proxied Domain Collection</span></span>

## <a name="properties"></a><span data-ttu-id="db845-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="db845-108">Properties</span></span>
|<span data-ttu-id="db845-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="db845-109">Property</span></span>|<span data-ttu-id="db845-110">Тип</span><span class="sxs-lookup"><span data-stu-id="db845-110">Type</span></span>|<span data-ttu-id="db845-111">Описание</span><span class="sxs-lookup"><span data-stu-id="db845-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db845-112">displayName</span><span class="sxs-lookup"><span data-stu-id="db845-112">displayName</span></span>|<span data-ttu-id="db845-113">Строка</span><span class="sxs-lookup"><span data-stu-id="db845-113">String</span></span>|<span data-ttu-id="db845-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="db845-114">Display name</span></span>|
|<span data-ttu-id="db845-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="db845-115">proxiedDomains</span></span>|<span data-ttu-id="db845-116">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="db845-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="db845-117">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="db845-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="db845-118">Связи</span><span class="sxs-lookup"><span data-stu-id="db845-118">Relationships</span></span>
<span data-ttu-id="db845-119">Нет</span><span class="sxs-lookup"><span data-stu-id="db845-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="db845-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="db845-120">JSON Representation</span></span>
<span data-ttu-id="db845-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="db845-121">Here is a JSON representation of the resource.</span></span>
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




