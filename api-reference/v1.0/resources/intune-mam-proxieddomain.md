---
title: Тип ресурса proxiedDomain
description: Проксируемый домен
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b28271308f5256d034de3b4704353aa0471aeb29
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465281"
---
# <a name="proxieddomain-resource-type"></a><span data-ttu-id="ce945-103">Тип ресурса proxiedDomain</span><span class="sxs-lookup"><span data-stu-id="ce945-103">proxiedDomain resource type</span></span>

> <span data-ttu-id="ce945-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce945-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce945-105">Проксируемый домен</span><span class="sxs-lookup"><span data-stu-id="ce945-105">Proxied Domain</span></span>

## <a name="properties"></a><span data-ttu-id="ce945-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce945-106">Properties</span></span>
|<span data-ttu-id="ce945-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce945-107">Property</span></span>|<span data-ttu-id="ce945-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ce945-108">Type</span></span>|<span data-ttu-id="ce945-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ce945-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce945-110">ipAddressOrFQDN</span><span class="sxs-lookup"><span data-stu-id="ce945-110">ipAddressOrFQDN</span></span>|<span data-ttu-id="ce945-111">Строка</span><span class="sxs-lookup"><span data-stu-id="ce945-111">String</span></span>|<span data-ttu-id="ce945-112">IP-адрес или полное доменное имя</span><span class="sxs-lookup"><span data-stu-id="ce945-112">The IP address or FQDN</span></span>|
|<span data-ttu-id="ce945-113">proxy</span><span class="sxs-lookup"><span data-stu-id="ce945-113">proxy</span></span>|<span data-ttu-id="ce945-114">Строка</span><span class="sxs-lookup"><span data-stu-id="ce945-114">String</span></span>|<span data-ttu-id="ce945-115">IP-адрес или полное ДОМЕНное имя прокси</span><span class="sxs-lookup"><span data-stu-id="ce945-115">Proxy IP or FQDN</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce945-116">Отношения</span><span class="sxs-lookup"><span data-stu-id="ce945-116">Relationships</span></span>
<span data-ttu-id="ce945-117">Нет</span><span class="sxs-lookup"><span data-stu-id="ce945-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce945-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce945-118">JSON Representation</span></span>
<span data-ttu-id="ce945-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce945-119">Here is a JSON representation of the resource.</span></span>
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



