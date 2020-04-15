---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6079a2503004a1606e9db0e4b20dce8725f37ab9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474105"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="453d2-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="453d2-103">proxiedDomain resource type</span></span>

<span data-ttu-id="453d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="453d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="453d2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="453d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="453d2-106">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="453d2-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="453d2-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="453d2-107">Properties</span></span>
|<span data-ttu-id="453d2-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="453d2-108">Property</span></span>|<span data-ttu-id="453d2-109">Тип</span><span class="sxs-lookup"><span data-stu-id="453d2-109">Type</span></span>|<span data-ttu-id="453d2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="453d2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="453d2-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="453d2-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="453d2-112">Строка</span><span class="sxs-lookup"><span data-stu-id="453d2-112">String</span></span>|<span data-ttu-id="453d2-113">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="453d2-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="453d2-114">proxy</span><span class="sxs-lookup"><span data-stu-id="453d2-114">proxy</span></span>|<span data-ttu-id="453d2-115">Строка</span><span class="sxs-lookup"><span data-stu-id="453d2-115">String</span></span>|<span data-ttu-id="453d2-116">IP-адрес или полное доменное имя прокси</span><span class="sxs-lookup"><span data-stu-id="453d2-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="453d2-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="453d2-117">Relationships</span></span>
<span data-ttu-id="453d2-118">Нет</span><span class="sxs-lookup"><span data-stu-id="453d2-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="453d2-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="453d2-119">JSON Representation</span></span>
<span data-ttu-id="453d2-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="453d2-120">Here is a JSON representation of the resource.</span></span>
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







