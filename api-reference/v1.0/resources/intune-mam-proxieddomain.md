---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25914b3cba48120e91352028bb51bcdee8edee2b
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752324"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="80dbf-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="80dbf-103">proxiedDomain resource type</span></span>

<span data-ttu-id="80dbf-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80dbf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80dbf-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="80dbf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80dbf-106">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="80dbf-106">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="80dbf-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="80dbf-107">Properties</span></span>
|<span data-ttu-id="80dbf-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="80dbf-108">Property</span></span>|<span data-ttu-id="80dbf-109">Тип</span><span class="sxs-lookup"><span data-stu-id="80dbf-109">Type</span></span>|<span data-ttu-id="80dbf-110">Описание</span><span class="sxs-lookup"><span data-stu-id="80dbf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80dbf-111">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="80dbf-111">ipAddressOrFQDN</span></span>|<span data-ttu-id="80dbf-112">Строка</span><span class="sxs-lookup"><span data-stu-id="80dbf-112">String</span></span>|<span data-ttu-id="80dbf-113">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="80dbf-113">The IP address or FQDN</span></span>|
|<span data-ttu-id="80dbf-114">proxy</span><span class="sxs-lookup"><span data-stu-id="80dbf-114">proxy</span></span>|<span data-ttu-id="80dbf-115">Строка</span><span class="sxs-lookup"><span data-stu-id="80dbf-115">String</span></span>|<span data-ttu-id="80dbf-116">IP-адрес прокси или FQDN</span><span class="sxs-lookup"><span data-stu-id="80dbf-116">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="80dbf-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="80dbf-117">Relationships</span></span>
<span data-ttu-id="80dbf-118">Нет</span><span class="sxs-lookup"><span data-stu-id="80dbf-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="80dbf-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="80dbf-119">JSON Representation</span></span>
<span data-ttu-id="80dbf-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="80dbf-120">Here is a JSON representation of the resource.</span></span>
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




