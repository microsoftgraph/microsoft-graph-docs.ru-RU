---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 352f466ad12f767feb68acd654d6d7d8133a25c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523592"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="6a133-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="6a133-103">proxiedDomain resource type</span></span>

<span data-ttu-id="6a133-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="6a133-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a133-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a133-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a133-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a133-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a133-107">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="6a133-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="6a133-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a133-108">Properties</span></span>
|<span data-ttu-id="6a133-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a133-109">Property</span></span>|<span data-ttu-id="6a133-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6a133-110">Type</span></span>|<span data-ttu-id="6a133-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6a133-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a133-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="6a133-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="6a133-113">Строка</span><span class="sxs-lookup"><span data-stu-id="6a133-113">String</span></span>|<span data-ttu-id="6a133-114">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="6a133-114">The IP address or FQDN</span></span>|
|<span data-ttu-id="6a133-115">proxy</span><span class="sxs-lookup"><span data-stu-id="6a133-115">proxy</span></span>|<span data-ttu-id="6a133-116">Строка</span><span class="sxs-lookup"><span data-stu-id="6a133-116">String</span></span>|<span data-ttu-id="6a133-117">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="6a133-117">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a133-118">Связи</span><span class="sxs-lookup"><span data-stu-id="6a133-118">Relationships</span></span>
<span data-ttu-id="6a133-119">Нет</span><span class="sxs-lookup"><span data-stu-id="6a133-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a133-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a133-120">JSON Representation</span></span>
<span data-ttu-id="6a133-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a133-121">Here is a JSON representation of the resource.</span></span>
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



