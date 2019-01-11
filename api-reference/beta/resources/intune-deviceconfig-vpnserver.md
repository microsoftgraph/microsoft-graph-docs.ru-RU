---
title: Тип ресурса vpnServer
description: Определение VPN-сервер.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b48daa95cc2227f6d1691902a75614446c93a10a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889875"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="38369-103">Тип ресурса vpnServer</span><span class="sxs-lookup"><span data-stu-id="38369-103">vpnServer resource type</span></span>

> <span data-ttu-id="38369-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="38369-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="38369-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="38369-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38369-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="38369-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38369-107">Определение VPN-сервер.</span><span class="sxs-lookup"><span data-stu-id="38369-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="38369-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="38369-108">Properties</span></span>
|<span data-ttu-id="38369-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="38369-109">Property</span></span>|<span data-ttu-id="38369-110">Тип</span><span class="sxs-lookup"><span data-stu-id="38369-110">Type</span></span>|<span data-ttu-id="38369-111">Описание</span><span class="sxs-lookup"><span data-stu-id="38369-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38369-112">описание</span><span class="sxs-lookup"><span data-stu-id="38369-112">description</span></span>|<span data-ttu-id="38369-113">Строка</span><span class="sxs-lookup"><span data-stu-id="38369-113">String</span></span>|<span data-ttu-id="38369-114">Описание.</span><span class="sxs-lookup"><span data-stu-id="38369-114">Description.</span></span>|
|<span data-ttu-id="38369-115">address</span><span class="sxs-lookup"><span data-stu-id="38369-115">address</span></span>|<span data-ttu-id="38369-116">String</span><span class="sxs-lookup"><span data-stu-id="38369-116">String</span></span>|<span data-ttu-id="38369-117">Адрес (IP-адрес, URL-адрес или полное доменное имя)</span><span class="sxs-lookup"><span data-stu-id="38369-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="38369-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="38369-118">isDefaultServer</span></span>|<span data-ttu-id="38369-119">Логический</span><span class="sxs-lookup"><span data-stu-id="38369-119">Boolean</span></span>|<span data-ttu-id="38369-120">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="38369-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38369-121">Связи</span><span class="sxs-lookup"><span data-stu-id="38369-121">Relationships</span></span>
<span data-ttu-id="38369-122">Нет</span><span class="sxs-lookup"><span data-stu-id="38369-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38369-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38369-123">JSON Representation</span></span>
<span data-ttu-id="38369-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38369-124">Here is a JSON representation of the resource.</span></span>
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





