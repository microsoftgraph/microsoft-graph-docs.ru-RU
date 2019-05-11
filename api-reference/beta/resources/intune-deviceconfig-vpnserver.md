---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67f0e91c0b2d024a07ab632a5e61e1106bbc65fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944529"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="79395-103">Тип ресурса Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="79395-103">vpnServer resource type</span></span>

> <span data-ttu-id="79395-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="79395-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="79395-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="79395-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79395-106">Определение VPN-сервера.</span><span class="sxs-lookup"><span data-stu-id="79395-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="79395-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="79395-107">Properties</span></span>
|<span data-ttu-id="79395-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="79395-108">Property</span></span>|<span data-ttu-id="79395-109">Тип</span><span class="sxs-lookup"><span data-stu-id="79395-109">Type</span></span>|<span data-ttu-id="79395-110">Описание</span><span class="sxs-lookup"><span data-stu-id="79395-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79395-111">description</span><span class="sxs-lookup"><span data-stu-id="79395-111">description</span></span>|<span data-ttu-id="79395-112">String</span><span class="sxs-lookup"><span data-stu-id="79395-112">String</span></span>|<span data-ttu-id="79395-113">Описание.</span><span class="sxs-lookup"><span data-stu-id="79395-113">Description.</span></span>|
|<span data-ttu-id="79395-114">address</span><span class="sxs-lookup"><span data-stu-id="79395-114">address</span></span>|<span data-ttu-id="79395-115">String</span><span class="sxs-lookup"><span data-stu-id="79395-115">String</span></span>|<span data-ttu-id="79395-116">Адрес (IP-адрес, полное ДОМЕНное имя или URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="79395-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="79395-117">Исдефаултсервер</span><span class="sxs-lookup"><span data-stu-id="79395-117">isDefaultServer</span></span>|<span data-ttu-id="79395-118">Логический</span><span class="sxs-lookup"><span data-stu-id="79395-118">Boolean</span></span>|<span data-ttu-id="79395-119">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="79395-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="79395-120">Связи</span><span class="sxs-lookup"><span data-stu-id="79395-120">Relationships</span></span>
<span data-ttu-id="79395-121">Нет</span><span class="sxs-lookup"><span data-stu-id="79395-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="79395-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="79395-122">JSON Representation</span></span>
<span data-ttu-id="79395-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="79395-123">Here is a JSON representation of the resource.</span></span>
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




