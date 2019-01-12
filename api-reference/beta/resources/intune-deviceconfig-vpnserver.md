---
title: Тип ресурса vpnServer
description: Определение VPN-сервер.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 61eaedb7ecca3f4a7074d079f2b10164dfe2ad76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969550"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="e0bf9-103">Тип ресурса vpnServer</span><span class="sxs-lookup"><span data-stu-id="e0bf9-103">vpnServer resource type</span></span>

> <span data-ttu-id="e0bf9-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e0bf9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e0bf9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e0bf9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e0bf9-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="e0bf9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0bf9-107">Определение VPN-сервер.</span><span class="sxs-lookup"><span data-stu-id="e0bf9-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="e0bf9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e0bf9-108">Properties</span></span>
|<span data-ttu-id="e0bf9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e0bf9-109">Property</span></span>|<span data-ttu-id="e0bf9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e0bf9-110">Type</span></span>|<span data-ttu-id="e0bf9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e0bf9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0bf9-112">описание</span><span class="sxs-lookup"><span data-stu-id="e0bf9-112">description</span></span>|<span data-ttu-id="e0bf9-113">Строка</span><span class="sxs-lookup"><span data-stu-id="e0bf9-113">String</span></span>|<span data-ttu-id="e0bf9-114">Описание.</span><span class="sxs-lookup"><span data-stu-id="e0bf9-114">Description.</span></span>|
|<span data-ttu-id="e0bf9-115">address</span><span class="sxs-lookup"><span data-stu-id="e0bf9-115">address</span></span>|<span data-ttu-id="e0bf9-116">String</span><span class="sxs-lookup"><span data-stu-id="e0bf9-116">String</span></span>|<span data-ttu-id="e0bf9-117">Адрес (IP-адрес, URL-адрес или полное доменное имя)</span><span class="sxs-lookup"><span data-stu-id="e0bf9-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="e0bf9-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="e0bf9-118">isDefaultServer</span></span>|<span data-ttu-id="e0bf9-119">Логический</span><span class="sxs-lookup"><span data-stu-id="e0bf9-119">Boolean</span></span>|<span data-ttu-id="e0bf9-120">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e0bf9-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0bf9-121">Связи</span><span class="sxs-lookup"><span data-stu-id="e0bf9-121">Relationships</span></span>
<span data-ttu-id="e0bf9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e0bf9-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e0bf9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e0bf9-123">JSON Representation</span></span>
<span data-ttu-id="e0bf9-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e0bf9-124">Here is a JSON representation of the resource.</span></span>
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





