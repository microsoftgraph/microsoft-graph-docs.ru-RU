---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 98b58759fbac16ad7fad78dc2a9ef0c449c42659
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554095"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="6a6bb-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="6a6bb-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="6a6bb-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6a6bb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a6bb-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6a6bb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a6bb-106">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="6a6bb-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="6a6bb-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a6bb-107">Properties</span></span>
|<span data-ttu-id="6a6bb-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a6bb-108">Property</span></span>|<span data-ttu-id="6a6bb-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6a6bb-109">Type</span></span>|<span data-ttu-id="6a6bb-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a6bb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a6bb-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="6a6bb-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="6a6bb-112">Строка</span><span class="sxs-lookup"><span data-stu-id="6a6bb-112">String</span></span>|<span data-ttu-id="6a6bb-113">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="6a6bb-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="6a6bb-114">proxy</span><span class="sxs-lookup"><span data-stu-id="6a6bb-114">proxy</span></span>|<span data-ttu-id="6a6bb-115">Строка</span><span class="sxs-lookup"><span data-stu-id="6a6bb-115">String</span></span>|<span data-ttu-id="6a6bb-116">IP-адрес или полное ДОМЕНное имя прокси</span><span class="sxs-lookup"><span data-stu-id="6a6bb-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a6bb-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="6a6bb-117">Relationships</span></span>
<span data-ttu-id="6a6bb-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6a6bb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a6bb-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a6bb-119">JSON Representation</span></span>
<span data-ttu-id="6a6bb-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a6bb-120">Here is a JSON representation of the resource.</span></span>
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





