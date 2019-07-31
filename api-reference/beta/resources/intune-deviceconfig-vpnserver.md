---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ead65c0657ebf999562899da5012d02fe7847a16
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969424"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="6d447-103">Тип ресурса Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="6d447-103">vpnServer resource type</span></span>

> <span data-ttu-id="6d447-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d447-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d447-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d447-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d447-106">Определение VPN-сервера.</span><span class="sxs-lookup"><span data-stu-id="6d447-106">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="6d447-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d447-107">Properties</span></span>
|<span data-ttu-id="6d447-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d447-108">Property</span></span>|<span data-ttu-id="6d447-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6d447-109">Type</span></span>|<span data-ttu-id="6d447-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6d447-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d447-111">description</span><span class="sxs-lookup"><span data-stu-id="6d447-111">description</span></span>|<span data-ttu-id="6d447-112">String</span><span class="sxs-lookup"><span data-stu-id="6d447-112">String</span></span>|<span data-ttu-id="6d447-113">Описание.</span><span class="sxs-lookup"><span data-stu-id="6d447-113">Description.</span></span>|
|<span data-ttu-id="6d447-114">address</span><span class="sxs-lookup"><span data-stu-id="6d447-114">address</span></span>|<span data-ttu-id="6d447-115">String</span><span class="sxs-lookup"><span data-stu-id="6d447-115">String</span></span>|<span data-ttu-id="6d447-116">Адрес (IP-адрес, полное доменное имя или URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="6d447-116">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="6d447-117">Исдефаултсервер</span><span class="sxs-lookup"><span data-stu-id="6d447-117">isDefaultServer</span></span>|<span data-ttu-id="6d447-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="6d447-118">Boolean</span></span>|<span data-ttu-id="6d447-119">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6d447-119">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d447-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="6d447-120">Relationships</span></span>
<span data-ttu-id="6d447-121">Нет</span><span class="sxs-lookup"><span data-stu-id="6d447-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d447-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d447-122">JSON Representation</span></span>
<span data-ttu-id="6d447-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d447-123">Here is a JSON representation of the resource.</span></span>
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





