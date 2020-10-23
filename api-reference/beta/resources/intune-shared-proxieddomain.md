---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ac366425621867e75dfc1a0c1ae8b09336ed0214
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704695"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="f9691-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="f9691-103">proxiedDomain resource type</span></span>

<span data-ttu-id="f9691-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9691-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f9691-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="f9691-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9691-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f9691-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9691-107">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="f9691-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="f9691-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="f9691-108">Properties</span></span>
|<span data-ttu-id="f9691-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="f9691-109">Property</span></span>|<span data-ttu-id="f9691-110">Тип</span><span class="sxs-lookup"><span data-stu-id="f9691-110">Type</span></span>|<span data-ttu-id="f9691-111">Описание</span><span class="sxs-lookup"><span data-stu-id="f9691-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9691-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="f9691-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="f9691-113">Строка</span><span class="sxs-lookup"><span data-stu-id="f9691-113">String</span></span>|<span data-ttu-id="f9691-114">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="f9691-114">The IP address or FQDN</span></span>|
|<span data-ttu-id="f9691-115">proxy</span><span class="sxs-lookup"><span data-stu-id="f9691-115">proxy</span></span>|<span data-ttu-id="f9691-116">Строка</span><span class="sxs-lookup"><span data-stu-id="f9691-116">String</span></span>|<span data-ttu-id="f9691-117">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="f9691-117">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9691-118">Связи</span><span class="sxs-lookup"><span data-stu-id="f9691-118">Relationships</span></span>
<span data-ttu-id="f9691-119">Нет</span><span class="sxs-lookup"><span data-stu-id="f9691-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9691-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f9691-120">JSON Representation</span></span>
<span data-ttu-id="f9691-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f9691-121">Here is a JSON representation of the resource.</span></span>
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





