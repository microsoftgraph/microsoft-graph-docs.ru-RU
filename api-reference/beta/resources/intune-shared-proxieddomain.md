---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b4b2dff399888ba51008f84b76decae8d211862e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466095"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="1021c-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="1021c-103">proxiedDomain resource type</span></span>

<span data-ttu-id="1021c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1021c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1021c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1021c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1021c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1021c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1021c-107">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="1021c-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="1021c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1021c-108">Properties</span></span>
|<span data-ttu-id="1021c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1021c-109">Property</span></span>|<span data-ttu-id="1021c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1021c-110">Type</span></span>|<span data-ttu-id="1021c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1021c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1021c-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="1021c-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="1021c-113">Строка</span><span class="sxs-lookup"><span data-stu-id="1021c-113">String</span></span>|<span data-ttu-id="1021c-114">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="1021c-114">The IP address or FQDN</span></span>|
|<span data-ttu-id="1021c-115">proxy</span><span class="sxs-lookup"><span data-stu-id="1021c-115">proxy</span></span>|<span data-ttu-id="1021c-116">Строка</span><span class="sxs-lookup"><span data-stu-id="1021c-116">String</span></span>|<span data-ttu-id="1021c-117">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="1021c-117">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="1021c-118">Связи</span><span class="sxs-lookup"><span data-stu-id="1021c-118">Relationships</span></span>
<span data-ttu-id="1021c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="1021c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1021c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1021c-120">JSON Representation</span></span>
<span data-ttu-id="1021c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1021c-121">Here is a JSON representation of the resource.</span></span>
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



