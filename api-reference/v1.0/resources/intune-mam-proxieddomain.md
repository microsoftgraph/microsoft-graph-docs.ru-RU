---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
ms.openlocfilehash: d73ed20341a7de025f6f2d39536a1e791b978f55
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27026945"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="e664c-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="e664c-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="e664c-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e664c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e664c-105">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="e664c-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="e664c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="e664c-106">Properties</span></span>
|<span data-ttu-id="e664c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="e664c-107">Property</span></span>|<span data-ttu-id="e664c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="e664c-108">Type</span></span>|<span data-ttu-id="e664c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="e664c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e664c-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="e664c-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="e664c-111">Строка</span><span class="sxs-lookup"><span data-stu-id="e664c-111">String</span></span>|<span data-ttu-id="e664c-112">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="e664c-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="e664c-113">proxy</span><span class="sxs-lookup"><span data-stu-id="e664c-113">proxy</span></span>|<span data-ttu-id="e664c-114">Строка</span><span class="sxs-lookup"><span data-stu-id="e664c-114">String</span></span>|<span data-ttu-id="e664c-115">IP-адрес прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="e664c-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="e664c-116">Связи</span><span class="sxs-lookup"><span data-stu-id="e664c-116">Relationships</span></span>
<span data-ttu-id="e664c-117">Нет</span><span class="sxs-lookup"><span data-stu-id="e664c-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e664c-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e664c-118">JSON Representation</span></span>
<span data-ttu-id="e664c-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e664c-119">Here is a JSON representation of the resource.</span></span>
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



