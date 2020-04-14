---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f687167b62e6b3a56f1deb76e3ee90c6ea7c62b7
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43420272"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="c1fa9-103">Тип ресурса Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="c1fa9-103">vpnServer resource type</span></span>

<span data-ttu-id="c1fa9-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1fa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c1fa9-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c1fa9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c1fa9-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c1fa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c1fa9-107">Определение VPN-сервера.</span><span class="sxs-lookup"><span data-stu-id="c1fa9-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="c1fa9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1fa9-108">Properties</span></span>
|<span data-ttu-id="c1fa9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1fa9-109">Property</span></span>|<span data-ttu-id="c1fa9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c1fa9-110">Type</span></span>|<span data-ttu-id="c1fa9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1fa9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1fa9-112">description</span><span class="sxs-lookup"><span data-stu-id="c1fa9-112">description</span></span>|<span data-ttu-id="c1fa9-113">String</span><span class="sxs-lookup"><span data-stu-id="c1fa9-113">String</span></span>|<span data-ttu-id="c1fa9-114">Описание.</span><span class="sxs-lookup"><span data-stu-id="c1fa9-114">Description.</span></span>|
|<span data-ttu-id="c1fa9-115">address</span><span class="sxs-lookup"><span data-stu-id="c1fa9-115">address</span></span>|<span data-ttu-id="c1fa9-116">String</span><span class="sxs-lookup"><span data-stu-id="c1fa9-116">String</span></span>|<span data-ttu-id="c1fa9-117">Адрес (IP-адрес, полное доменное имя или URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="c1fa9-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="c1fa9-118">исдефаултсервер</span><span class="sxs-lookup"><span data-stu-id="c1fa9-118">isDefaultServer</span></span>|<span data-ttu-id="c1fa9-119">Логическое</span><span class="sxs-lookup"><span data-stu-id="c1fa9-119">Boolean</span></span>|<span data-ttu-id="c1fa9-120">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="c1fa9-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1fa9-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c1fa9-121">Relationships</span></span>
<span data-ttu-id="c1fa9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c1fa9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1fa9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1fa9-123">JSON Representation</span></span>
<span data-ttu-id="c1fa9-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1fa9-124">Here is a JSON representation of the resource.</span></span>
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



