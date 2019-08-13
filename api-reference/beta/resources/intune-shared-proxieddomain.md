---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e44a6208aab688e566d89a9dce84b21e65c3c284
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347859"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="be27f-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="be27f-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="be27f-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="be27f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be27f-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="be27f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be27f-106">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="be27f-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="be27f-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="be27f-107">Properties</span></span>
|<span data-ttu-id="be27f-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="be27f-108">Property</span></span>|<span data-ttu-id="be27f-109">Тип</span><span class="sxs-lookup"><span data-stu-id="be27f-109">Type</span></span>|<span data-ttu-id="be27f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="be27f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be27f-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="be27f-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="be27f-112">Строка</span><span class="sxs-lookup"><span data-stu-id="be27f-112">String</span></span>|<span data-ttu-id="be27f-113">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="be27f-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="be27f-114">proxy</span><span class="sxs-lookup"><span data-stu-id="be27f-114">proxy</span></span>|<span data-ttu-id="be27f-115">Строка</span><span class="sxs-lookup"><span data-stu-id="be27f-115">String</span></span>|<span data-ttu-id="be27f-116">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="be27f-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="be27f-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="be27f-117">Relationships</span></span>
<span data-ttu-id="be27f-118">Нет</span><span class="sxs-lookup"><span data-stu-id="be27f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be27f-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="be27f-119">JSON Representation</span></span>
<span data-ttu-id="be27f-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="be27f-120">Here is a JSON representation of the resource.</span></span>
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



