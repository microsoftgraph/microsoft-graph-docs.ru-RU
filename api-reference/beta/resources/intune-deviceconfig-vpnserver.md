---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 577b606ee4dc46cd5ed8f93c351f5b41e73fe973
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787322"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="d6bf6-103">Тип ресурса Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="d6bf6-103">vpnServer resource type</span></span>

> <span data-ttu-id="d6bf6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6bf6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6bf6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d6bf6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6bf6-106">Определение VPN-сервера.</span><span class="sxs-lookup"><span data-stu-id="d6bf6-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d6bf6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6bf6-107">Properties</span></span>
|<span data-ttu-id="d6bf6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6bf6-108">Property</span></span>|<span data-ttu-id="d6bf6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d6bf6-109">Type</span></span>|<span data-ttu-id="d6bf6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d6bf6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bf6-111">description</span><span class="sxs-lookup"><span data-stu-id="d6bf6-111">description</span></span>|<span data-ttu-id="d6bf6-112">String</span><span class="sxs-lookup"><span data-stu-id="d6bf6-112">String</span></span>|<span data-ttu-id="d6bf6-113">Описание.</span><span class="sxs-lookup"><span data-stu-id="d6bf6-113">Description.</span></span>|
|<span data-ttu-id="d6bf6-114">address</span><span class="sxs-lookup"><span data-stu-id="d6bf6-114">address</span></span>|<span data-ttu-id="d6bf6-115">String</span><span class="sxs-lookup"><span data-stu-id="d6bf6-115">String</span></span>|<span data-ttu-id="d6bf6-116">Адрес (IP-адрес, полное доменное имя или URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="d6bf6-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="d6bf6-117">исдефаултсервер</span><span class="sxs-lookup"><span data-stu-id="d6bf6-117">isDefaultServer</span></span>|<span data-ttu-id="d6bf6-118">Логический</span><span class="sxs-lookup"><span data-stu-id="d6bf6-118">Boolean</span></span>|<span data-ttu-id="d6bf6-119">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d6bf6-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6bf6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="d6bf6-120">Relationships</span></span>
<span data-ttu-id="d6bf6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="d6bf6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d6bf6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6bf6-122">JSON Representation</span></span>
<span data-ttu-id="d6bf6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6bf6-123">Here is a JSON representation of the resource.</span></span>
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



