---
title: Тип ресурса vpnServer
description: Определение VPN-сервер.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 0febdae5745f1295e9c690213d4a51b79d7d3bdb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406810"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="35e52-103">Тип ресурса vpnServer</span><span class="sxs-lookup"><span data-stu-id="35e52-103">vpnServer resource type</span></span>

> <span data-ttu-id="35e52-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="35e52-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="35e52-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="35e52-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="35e52-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="35e52-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35e52-107">Определение VPN-сервер.</span><span class="sxs-lookup"><span data-stu-id="35e52-107">VPN Server definition.</span></span>

## <a name="properties"></a><span data-ttu-id="35e52-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="35e52-108">Properties</span></span>
|<span data-ttu-id="35e52-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="35e52-109">Property</span></span>|<span data-ttu-id="35e52-110">Тип</span><span class="sxs-lookup"><span data-stu-id="35e52-110">Type</span></span>|<span data-ttu-id="35e52-111">Описание</span><span class="sxs-lookup"><span data-stu-id="35e52-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35e52-112">description</span><span class="sxs-lookup"><span data-stu-id="35e52-112">description</span></span>|<span data-ttu-id="35e52-113">String</span><span class="sxs-lookup"><span data-stu-id="35e52-113">String</span></span>|<span data-ttu-id="35e52-114">Описание.</span><span class="sxs-lookup"><span data-stu-id="35e52-114">Description.</span></span>|
|<span data-ttu-id="35e52-115">address</span><span class="sxs-lookup"><span data-stu-id="35e52-115">address</span></span>|<span data-ttu-id="35e52-116">String</span><span class="sxs-lookup"><span data-stu-id="35e52-116">String</span></span>|<span data-ttu-id="35e52-117">Адрес (IP-адрес, URL-адрес или полное доменное имя)</span><span class="sxs-lookup"><span data-stu-id="35e52-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="35e52-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="35e52-118">isDefaultServer</span></span>|<span data-ttu-id="35e52-119">Логический</span><span class="sxs-lookup"><span data-stu-id="35e52-119">Boolean</span></span>|<span data-ttu-id="35e52-120">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="35e52-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35e52-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="35e52-121">Relationships</span></span>
<span data-ttu-id="35e52-122">Нет</span><span class="sxs-lookup"><span data-stu-id="35e52-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35e52-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="35e52-123">JSON Representation</span></span>
<span data-ttu-id="35e52-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="35e52-124">Here is a JSON representation of the resource.</span></span>
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




