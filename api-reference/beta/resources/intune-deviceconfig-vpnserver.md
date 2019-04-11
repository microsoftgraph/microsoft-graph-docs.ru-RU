---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0bf45848059f7cbd74b408b4074b0ebc5c31b4e5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782837"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="e52e5-103">Тип ресурса Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="e52e5-103">vpnServer resource type</span></span>

> <span data-ttu-id="e52e5-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e52e5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e52e5-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e52e5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e52e5-106">Определение VPN-сервера.</span><span class="sxs-lookup"><span data-stu-id="e52e5-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="e52e5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e52e5-107">Properties</span></span>
|<span data-ttu-id="e52e5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e52e5-108">Property</span></span>|<span data-ttu-id="e52e5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e52e5-109">Type</span></span>|<span data-ttu-id="e52e5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e52e5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e52e5-111">description</span><span class="sxs-lookup"><span data-stu-id="e52e5-111">description</span></span>|<span data-ttu-id="e52e5-112">String</span><span class="sxs-lookup"><span data-stu-id="e52e5-112">String</span></span>|<span data-ttu-id="e52e5-113">Описание.</span><span class="sxs-lookup"><span data-stu-id="e52e5-113">Description.</span></span>|
|<span data-ttu-id="e52e5-114">address</span><span class="sxs-lookup"><span data-stu-id="e52e5-114">address</span></span>|<span data-ttu-id="e52e5-115">String</span><span class="sxs-lookup"><span data-stu-id="e52e5-115">String</span></span>|<span data-ttu-id="e52e5-116">Адрес (IP-адрес, полное ДОМЕНное имя или URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="e52e5-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="e52e5-117">Исдефаултсервер</span><span class="sxs-lookup"><span data-stu-id="e52e5-117">isDefaultServer</span></span>|<span data-ttu-id="e52e5-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="e52e5-118">Boolean</span></span>|<span data-ttu-id="e52e5-119">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e52e5-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e52e5-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="e52e5-120">Relationships</span></span>
<span data-ttu-id="e52e5-121">Нет</span><span class="sxs-lookup"><span data-stu-id="e52e5-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e52e5-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e52e5-122">JSON Representation</span></span>
<span data-ttu-id="e52e5-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e52e5-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```





