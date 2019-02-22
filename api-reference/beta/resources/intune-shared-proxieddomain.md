---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5edabc31761a3abd79a94bb700392923d2d54513
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151207"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="bc12c-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="bc12c-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="bc12c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bc12c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc12c-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bc12c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc12c-106">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="bc12c-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="bc12c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="bc12c-107">Properties</span></span>
|<span data-ttu-id="bc12c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="bc12c-108">Property</span></span>|<span data-ttu-id="bc12c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="bc12c-109">Type</span></span>|<span data-ttu-id="bc12c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="bc12c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc12c-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="bc12c-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="bc12c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="bc12c-112">String</span></span>|<span data-ttu-id="bc12c-113">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="bc12c-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="bc12c-114">proxy</span><span class="sxs-lookup"><span data-stu-id="bc12c-114">proxy</span></span>|<span data-ttu-id="bc12c-115">Строка</span><span class="sxs-lookup"><span data-stu-id="bc12c-115">String</span></span>|<span data-ttu-id="bc12c-116">IP-адрес или полное ДОМЕНное имя прокси</span><span class="sxs-lookup"><span data-stu-id="bc12c-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc12c-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="bc12c-117">Relationships</span></span>
<span data-ttu-id="bc12c-118">Нет</span><span class="sxs-lookup"><span data-stu-id="bc12c-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc12c-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bc12c-119">JSON Representation</span></span>
<span data-ttu-id="bc12c-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bc12c-120">Here is a JSON representation of the resource.</span></span>
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




