---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dc90ebd57752fedcaf7acf069da6e653da04978e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968549"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="6ce00-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="6ce00-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="6ce00-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="6ce00-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ce00-105">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="6ce00-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="6ce00-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6ce00-106">Properties</span></span>
|<span data-ttu-id="6ce00-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6ce00-107">Property</span></span>|<span data-ttu-id="6ce00-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6ce00-108">Type</span></span>|<span data-ttu-id="6ce00-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6ce00-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ce00-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="6ce00-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="6ce00-111">Строка</span><span class="sxs-lookup"><span data-stu-id="6ce00-111">String</span></span>|<span data-ttu-id="6ce00-112">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="6ce00-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="6ce00-113">proxy</span><span class="sxs-lookup"><span data-stu-id="6ce00-113">proxy</span></span>|<span data-ttu-id="6ce00-114">Строка</span><span class="sxs-lookup"><span data-stu-id="6ce00-114">String</span></span>|<span data-ttu-id="6ce00-115">IP-адрес прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="6ce00-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ce00-116">Связи</span><span class="sxs-lookup"><span data-stu-id="6ce00-116">Relationships</span></span>
<span data-ttu-id="6ce00-117">Нет</span><span class="sxs-lookup"><span data-stu-id="6ce00-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6ce00-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6ce00-118">JSON Representation</span></span>
<span data-ttu-id="6ce00-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6ce00-119">Here is a JSON representation of the resource.</span></span>
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



