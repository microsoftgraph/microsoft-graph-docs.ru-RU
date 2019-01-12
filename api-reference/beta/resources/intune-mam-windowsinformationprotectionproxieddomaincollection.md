---
title: Тип ресурса windowsInformationProtectionProxiedDomainCollection
description: Коллекция проксируемых доменов Windows Information Protection
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a2f4b1e29afd113c2e06b611fabd525f9f5a6ba1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916904"
---
# <a name="windowsinformationprotectionproxieddomaincollection-resource-type"></a><span data-ttu-id="564cf-103">Тип ресурса windowsInformationProtectionProxiedDomainCollection</span><span class="sxs-lookup"><span data-stu-id="564cf-103">windowsInformationProtectionProxiedDomainCollection resource type</span></span>

> <span data-ttu-id="564cf-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="564cf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="564cf-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="564cf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="564cf-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="564cf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="564cf-107">Коллекция проксируемых доменов Windows Information Protection</span><span class="sxs-lookup"><span data-stu-id="564cf-107">Windows Information Protection Proxied Domain Collection</span></span>
## <a name="properties"></a><span data-ttu-id="564cf-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="564cf-108">Properties</span></span>
|<span data-ttu-id="564cf-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="564cf-109">Property</span></span>|<span data-ttu-id="564cf-110">Тип</span><span class="sxs-lookup"><span data-stu-id="564cf-110">Type</span></span>|<span data-ttu-id="564cf-111">Описание</span><span class="sxs-lookup"><span data-stu-id="564cf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="564cf-112">displayName</span><span class="sxs-lookup"><span data-stu-id="564cf-112">displayName</span></span>|<span data-ttu-id="564cf-113">Строка</span><span class="sxs-lookup"><span data-stu-id="564cf-113">String</span></span>|<span data-ttu-id="564cf-114">Отображаемое имя</span><span class="sxs-lookup"><span data-stu-id="564cf-114">Display name</span></span>|
|<span data-ttu-id="564cf-115">proxiedDomains</span><span class="sxs-lookup"><span data-stu-id="564cf-115">proxiedDomains</span></span>|<span data-ttu-id="564cf-116">Коллекция объектов [proxiedDomain](../resources/intune-shared-proxieddomain.md)</span><span class="sxs-lookup"><span data-stu-id="564cf-116">[proxiedDomain](../resources/intune-shared-proxieddomain.md) collection</span></span>|<span data-ttu-id="564cf-117">Коллекция проксируемых доменов</span><span class="sxs-lookup"><span data-stu-id="564cf-117">Collection of proxied domains</span></span>|

## <a name="relationships"></a><span data-ttu-id="564cf-118">Связи</span><span class="sxs-lookup"><span data-stu-id="564cf-118">Relationships</span></span>
<span data-ttu-id="564cf-119">Нет</span><span class="sxs-lookup"><span data-stu-id="564cf-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="564cf-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="564cf-120">JSON Representation</span></span>
<span data-ttu-id="564cf-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="564cf-121">Here is a JSON representation of the resource.</span></span>
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





