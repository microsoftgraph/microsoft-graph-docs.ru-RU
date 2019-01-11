---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: eff345414531b0ddda1600bb567aacd4a5436602
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871115"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="433be-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="433be-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="433be-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="433be-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="433be-105">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="433be-105">Proxied Domain</span></span>
## <a name="properties"></a><span data-ttu-id="433be-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="433be-106">Properties</span></span>
|<span data-ttu-id="433be-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="433be-107">Property</span></span>|<span data-ttu-id="433be-108">Тип</span><span class="sxs-lookup"><span data-stu-id="433be-108">Type</span></span>|<span data-ttu-id="433be-109">Описание</span><span class="sxs-lookup"><span data-stu-id="433be-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="433be-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="433be-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="433be-111">Строка</span><span class="sxs-lookup"><span data-stu-id="433be-111">String</span></span>|<span data-ttu-id="433be-112">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="433be-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="433be-113">proxy</span><span class="sxs-lookup"><span data-stu-id="433be-113">proxy</span></span>|<span data-ttu-id="433be-114">Строка</span><span class="sxs-lookup"><span data-stu-id="433be-114">String</span></span>|<span data-ttu-id="433be-115">IP-адрес прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="433be-115">Proxy IP</span></span>|

## <a name="relationships"></a><span data-ttu-id="433be-116">Связи</span><span class="sxs-lookup"><span data-stu-id="433be-116">Relationships</span></span>
<span data-ttu-id="433be-117">Нет</span><span class="sxs-lookup"><span data-stu-id="433be-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="433be-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="433be-118">JSON Representation</span></span>
<span data-ttu-id="433be-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="433be-119">Here is a JSON representation of the resource.</span></span>
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



