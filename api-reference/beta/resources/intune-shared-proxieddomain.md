---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d0b5f347081c0e2bb19ced382ed24faad1f7837
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33938606"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="8c0e5-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="8c0e5-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="8c0e5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8c0e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c0e5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8c0e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c0e5-106">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="8c0e5-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="8c0e5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c0e5-107">Properties</span></span>
|<span data-ttu-id="8c0e5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c0e5-108">Property</span></span>|<span data-ttu-id="8c0e5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="8c0e5-109">Type</span></span>|<span data-ttu-id="8c0e5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8c0e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c0e5-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="8c0e5-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="8c0e5-112">Строка</span><span class="sxs-lookup"><span data-stu-id="8c0e5-112">String</span></span>|<span data-ttu-id="8c0e5-113">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="8c0e5-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="8c0e5-114">proxy</span><span class="sxs-lookup"><span data-stu-id="8c0e5-114">proxy</span></span>|<span data-ttu-id="8c0e5-115">Строка</span><span class="sxs-lookup"><span data-stu-id="8c0e5-115">String</span></span>|<span data-ttu-id="8c0e5-116">IP-адрес или полное ДОМЕНное имя прокси</span><span class="sxs-lookup"><span data-stu-id="8c0e5-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c0e5-117">Связи</span><span class="sxs-lookup"><span data-stu-id="8c0e5-117">Relationships</span></span>
<span data-ttu-id="8c0e5-118">Нет</span><span class="sxs-lookup"><span data-stu-id="8c0e5-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c0e5-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c0e5-119">JSON Representation</span></span>
<span data-ttu-id="8c0e5-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c0e5-120">Here is a JSON representation of the resource.</span></span>
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




