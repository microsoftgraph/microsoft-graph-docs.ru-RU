---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b25d40058f4f79add5875698777e23f658992e05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846776"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="bb61b-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="bb61b-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="bb61b-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb61b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bb61b-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb61b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb61b-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="bb61b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bb61b-107">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="bb61b-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="bb61b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb61b-108">Properties</span></span>
|<span data-ttu-id="bb61b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb61b-109">Property</span></span>|<span data-ttu-id="bb61b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bb61b-110">Type</span></span>|<span data-ttu-id="bb61b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bb61b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb61b-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="bb61b-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="bb61b-113">Строка</span><span class="sxs-lookup"><span data-stu-id="bb61b-113">String</span></span>|<span data-ttu-id="bb61b-114">IP-адрес или полное доменное имя (FQDN).</span><span class="sxs-lookup"><span data-stu-id="bb61b-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="bb61b-115">proxy</span><span class="sxs-lookup"><span data-stu-id="bb61b-115">proxy</span></span>|<span data-ttu-id="bb61b-116">Строка</span><span class="sxs-lookup"><span data-stu-id="bb61b-116">String</span></span>|<span data-ttu-id="bb61b-117">IP-адрес прокси-сервера или полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="bb61b-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb61b-118">Связи</span><span class="sxs-lookup"><span data-stu-id="bb61b-118">Relationships</span></span>
<span data-ttu-id="bb61b-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bb61b-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb61b-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb61b-120">JSON Representation</span></span>
<span data-ttu-id="bb61b-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb61b-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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



