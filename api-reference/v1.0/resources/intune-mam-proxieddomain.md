---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e7530bf3bc08deded241257a9c787698682cd9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037830"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="295fd-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="295fd-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="295fd-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="295fd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="295fd-105">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="295fd-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="295fd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="295fd-106">Properties</span></span>
|<span data-ttu-id="295fd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="295fd-107">Property</span></span>|<span data-ttu-id="295fd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="295fd-108">Type</span></span>|<span data-ttu-id="295fd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="295fd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="295fd-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="295fd-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="295fd-111">Строка</span><span class="sxs-lookup"><span data-stu-id="295fd-111">String</span></span>|<span data-ttu-id="295fd-112">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="295fd-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="295fd-113">proxy</span><span class="sxs-lookup"><span data-stu-id="295fd-113">proxy</span></span>|<span data-ttu-id="295fd-114">Строка</span><span class="sxs-lookup"><span data-stu-id="295fd-114">String</span></span>|<span data-ttu-id="295fd-115">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="295fd-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="295fd-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="295fd-116">Relationships</span></span>
<span data-ttu-id="295fd-117">Нет</span><span class="sxs-lookup"><span data-stu-id="295fd-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="295fd-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="295fd-118">JSON Representation</span></span>
<span data-ttu-id="295fd-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="295fd-119">Here is a JSON representation of the resource.</span></span>
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



