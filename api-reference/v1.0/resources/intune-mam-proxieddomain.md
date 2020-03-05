---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e437c6bf035d0f6099531fbe5ebf236d30be3a2f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448279"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="2ee2b-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="2ee2b-103">proxiedDomain resource type</span></span>

<span data-ttu-id="2ee2b-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2ee2b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ee2b-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ee2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ee2b-106">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="2ee2b-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="2ee2b-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ee2b-107">Properties</span></span>
|<span data-ttu-id="2ee2b-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ee2b-108">Property</span></span>|<span data-ttu-id="2ee2b-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ee2b-109">Type</span></span>|<span data-ttu-id="2ee2b-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ee2b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ee2b-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="2ee2b-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="2ee2b-112">Строка</span><span class="sxs-lookup"><span data-stu-id="2ee2b-112">String</span></span>|<span data-ttu-id="2ee2b-113">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="2ee2b-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="2ee2b-114">proxy</span><span class="sxs-lookup"><span data-stu-id="2ee2b-114">proxy</span></span>|<span data-ttu-id="2ee2b-115">Строка</span><span class="sxs-lookup"><span data-stu-id="2ee2b-115">String</span></span>|<span data-ttu-id="2ee2b-116">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="2ee2b-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ee2b-117">Связи</span><span class="sxs-lookup"><span data-stu-id="2ee2b-117">Relationships</span></span>
<span data-ttu-id="2ee2b-118">Нет</span><span class="sxs-lookup"><span data-stu-id="2ee2b-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ee2b-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ee2b-119">JSON Representation</span></span>
<span data-ttu-id="2ee2b-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ee2b-120">Here is a JSON representation of the resource.</span></span>
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




