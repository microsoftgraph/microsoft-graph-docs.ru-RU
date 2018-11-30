---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
ms.openlocfilehash: 310ccb1420ed450c9e7c53d534181720f9051ff4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27075845"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="150e9-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="150e9-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="150e9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="150e9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="150e9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="150e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="150e9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="150e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="150e9-107">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="150e9-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="150e9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="150e9-108">Properties</span></span>
|<span data-ttu-id="150e9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="150e9-109">Property</span></span>|<span data-ttu-id="150e9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="150e9-110">Type</span></span>|<span data-ttu-id="150e9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="150e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="150e9-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="150e9-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="150e9-113">Строка</span><span class="sxs-lookup"><span data-stu-id="150e9-113">String</span></span>|<span data-ttu-id="150e9-114">IP-адрес или полное доменное имя (FQDN).</span><span class="sxs-lookup"><span data-stu-id="150e9-114">The IP address or fully qualified domain name (FQDN).</span></span>|
|<span data-ttu-id="150e9-115">proxy</span><span class="sxs-lookup"><span data-stu-id="150e9-115">proxy</span></span>|<span data-ttu-id="150e9-116">Строка</span><span class="sxs-lookup"><span data-stu-id="150e9-116">String</span></span>|<span data-ttu-id="150e9-117">IP-адрес прокси-сервера или полное доменное имя.</span><span class="sxs-lookup"><span data-stu-id="150e9-117">Proxy IP address or FQDN.</span></span>|

## <a name="relationships"></a><span data-ttu-id="150e9-118">Связи</span><span class="sxs-lookup"><span data-stu-id="150e9-118">Relationships</span></span>
<span data-ttu-id="150e9-119">Нет</span><span class="sxs-lookup"><span data-stu-id="150e9-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="150e9-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="150e9-120">JSON Representation</span></span>
<span data-ttu-id="150e9-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="150e9-121">Here is a JSON representation of the resource.</span></span>
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



