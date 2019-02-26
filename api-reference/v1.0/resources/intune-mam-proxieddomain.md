---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b28271308f5256d034de3b4704353aa0471aeb29
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264045"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="ad7f2-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="ad7f2-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="ad7f2-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ad7f2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ad7f2-105">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="ad7f2-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="ad7f2-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad7f2-106">Properties</span></span>
|<span data-ttu-id="ad7f2-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad7f2-107">Property</span></span>|<span data-ttu-id="ad7f2-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ad7f2-108">Type</span></span>|<span data-ttu-id="ad7f2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ad7f2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad7f2-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="ad7f2-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="ad7f2-111">Строка</span><span class="sxs-lookup"><span data-stu-id="ad7f2-111">String</span></span>|<span data-ttu-id="ad7f2-112">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="ad7f2-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="ad7f2-113">proxy</span><span class="sxs-lookup"><span data-stu-id="ad7f2-113">proxy</span></span>|<span data-ttu-id="ad7f2-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ad7f2-114">String</span></span>|<span data-ttu-id="ad7f2-115">IP-адрес или полное ДОМЕНное имя прокси</span><span class="sxs-lookup"><span data-stu-id="ad7f2-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad7f2-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="ad7f2-116">Relationships</span></span>
<span data-ttu-id="ad7f2-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ad7f2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad7f2-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ad7f2-118">JSON Representation</span></span>
<span data-ttu-id="ad7f2-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad7f2-119">Here is a JSON representation of the resource.</span></span>
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



