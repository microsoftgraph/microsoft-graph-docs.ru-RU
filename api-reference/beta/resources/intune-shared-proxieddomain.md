---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bdfdf1fdbea81f415633c810bd21172164f3765f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42768060"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="61965-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="61965-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="61965-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="61965-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61965-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="61965-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61965-106">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="61965-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="61965-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="61965-107">Properties</span></span>
|<span data-ttu-id="61965-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="61965-108">Property</span></span>|<span data-ttu-id="61965-109">Тип</span><span class="sxs-lookup"><span data-stu-id="61965-109">Type</span></span>|<span data-ttu-id="61965-110">Описание</span><span class="sxs-lookup"><span data-stu-id="61965-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61965-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="61965-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="61965-112">Строка</span><span class="sxs-lookup"><span data-stu-id="61965-112">String</span></span>|<span data-ttu-id="61965-113">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="61965-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="61965-114">proxy</span><span class="sxs-lookup"><span data-stu-id="61965-114">proxy</span></span>|<span data-ttu-id="61965-115">Строка</span><span class="sxs-lookup"><span data-stu-id="61965-115">String</span></span>|<span data-ttu-id="61965-116">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="61965-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="61965-117">Связи</span><span class="sxs-lookup"><span data-stu-id="61965-117">Relationships</span></span>
<span data-ttu-id="61965-118">Нет</span><span class="sxs-lookup"><span data-stu-id="61965-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="61965-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="61965-119">JSON Representation</span></span>
<span data-ttu-id="61965-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="61965-120">Here is a JSON representation of the resource.</span></span>
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



