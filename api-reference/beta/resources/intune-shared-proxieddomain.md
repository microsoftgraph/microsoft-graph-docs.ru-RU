---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b31786ac628d1f1abab5309f1ae327909dac7076
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49258880"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="d12bd-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="d12bd-103">proxiedDomain resource type</span></span>

<span data-ttu-id="d12bd-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d12bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d12bd-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d12bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d12bd-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d12bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d12bd-107">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="d12bd-107">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="d12bd-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d12bd-108">Properties</span></span>
|<span data-ttu-id="d12bd-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d12bd-109">Property</span></span>|<span data-ttu-id="d12bd-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d12bd-110">Type</span></span>|<span data-ttu-id="d12bd-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d12bd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d12bd-112">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="d12bd-112">ipAddressOrFQDN</span></span>|<span data-ttu-id="d12bd-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d12bd-113">String</span></span>|<span data-ttu-id="d12bd-114">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="d12bd-114">The IP address or FQDN</span></span>|
|<span data-ttu-id="d12bd-115">proxy</span><span class="sxs-lookup"><span data-stu-id="d12bd-115">proxy</span></span>|<span data-ttu-id="d12bd-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d12bd-116">String</span></span>|<span data-ttu-id="d12bd-117">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="d12bd-117">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="d12bd-118">Связи</span><span class="sxs-lookup"><span data-stu-id="d12bd-118">Relationships</span></span>
<span data-ttu-id="d12bd-119">Нет</span><span class="sxs-lookup"><span data-stu-id="d12bd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d12bd-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d12bd-120">JSON Representation</span></span>
<span data-ttu-id="d12bd-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d12bd-121">Here is a JSON representation of the resource.</span></span>
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




