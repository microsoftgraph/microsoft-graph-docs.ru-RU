---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8d4b100fd312576fdb81f09e06b51d7e74bef4c0
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366960"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="c626b-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="c626b-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="c626b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c626b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c626b-105">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="c626b-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="c626b-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c626b-106">Properties</span></span>
|<span data-ttu-id="c626b-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c626b-107">Property</span></span>|<span data-ttu-id="c626b-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c626b-108">Type</span></span>|<span data-ttu-id="c626b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c626b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c626b-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="c626b-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="c626b-111">Строка</span><span class="sxs-lookup"><span data-stu-id="c626b-111">String</span></span>|<span data-ttu-id="c626b-112">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="c626b-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="c626b-113">proxy</span><span class="sxs-lookup"><span data-stu-id="c626b-113">proxy</span></span>|<span data-ttu-id="c626b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="c626b-114">String</span></span>|<span data-ttu-id="c626b-115">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="c626b-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="c626b-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c626b-116">Relationships</span></span>
<span data-ttu-id="c626b-117">Нет</span><span class="sxs-lookup"><span data-stu-id="c626b-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c626b-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c626b-118">JSON Representation</span></span>
<span data-ttu-id="c626b-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c626b-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.proxiedDomain"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.proxiedDomain",
  "ipAddressOrFQDN": "String",
  "proxy": "String"
}
```




