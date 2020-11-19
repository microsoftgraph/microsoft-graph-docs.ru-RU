---
title: Тип ресурса Vpnserver.
description: Определение VPN-сервера.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8281aaaec193b5a78e913af52ce51d8f327ce8cf
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279481"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="222eb-103">Тип ресурса Vpnserver.</span><span class="sxs-lookup"><span data-stu-id="222eb-103">vpnServer resource type</span></span>

<span data-ttu-id="222eb-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="222eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="222eb-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="222eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="222eb-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="222eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="222eb-107">Определение VPN-сервера.</span><span class="sxs-lookup"><span data-stu-id="222eb-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="222eb-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="222eb-108">Properties</span></span>
|<span data-ttu-id="222eb-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="222eb-109">Property</span></span>|<span data-ttu-id="222eb-110">Тип</span><span class="sxs-lookup"><span data-stu-id="222eb-110">Type</span></span>|<span data-ttu-id="222eb-111">Описание</span><span class="sxs-lookup"><span data-stu-id="222eb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="222eb-112">description</span><span class="sxs-lookup"><span data-stu-id="222eb-112">description</span></span>|<span data-ttu-id="222eb-113">String</span><span class="sxs-lookup"><span data-stu-id="222eb-113">String</span></span>|<span data-ttu-id="222eb-114">Описание.</span><span class="sxs-lookup"><span data-stu-id="222eb-114">Description.</span></span>|
|<span data-ttu-id="222eb-115">address</span><span class="sxs-lookup"><span data-stu-id="222eb-115">address</span></span>|<span data-ttu-id="222eb-116">String</span><span class="sxs-lookup"><span data-stu-id="222eb-116">String</span></span>|<span data-ttu-id="222eb-117">Адрес (IP-адрес, полное доменное имя или URL-адрес)</span><span class="sxs-lookup"><span data-stu-id="222eb-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="222eb-118">исдефаултсервер</span><span class="sxs-lookup"><span data-stu-id="222eb-118">isDefaultServer</span></span>|<span data-ttu-id="222eb-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="222eb-119">Boolean</span></span>|<span data-ttu-id="222eb-120">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="222eb-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="222eb-121">Связи</span><span class="sxs-lookup"><span data-stu-id="222eb-121">Relationships</span></span>
<span data-ttu-id="222eb-122">Нет</span><span class="sxs-lookup"><span data-stu-id="222eb-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="222eb-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="222eb-123">JSON Representation</span></span>
<span data-ttu-id="222eb-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="222eb-124">Here is a JSON representation of the resource.</span></span>
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




