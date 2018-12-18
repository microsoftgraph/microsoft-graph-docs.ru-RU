---
title: Тип ресурса vpnServer
description: Определение VPN-сервер.
author: tfitzmac
ms.openlocfilehash: a8f0e6bd38f243d0066da231ef07d1723961987b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328779"
---
# <a name="vpnserver-resource-type"></a><span data-ttu-id="d1169-103">Тип ресурса vpnServer</span><span class="sxs-lookup"><span data-stu-id="d1169-103">vpnServer resource type</span></span>

> <span data-ttu-id="d1169-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d1169-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1169-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d1169-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1169-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d1169-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1169-107">Определение VPN-сервер.</span><span class="sxs-lookup"><span data-stu-id="d1169-107">VPN Server definition.</span></span>
## <a name="properties"></a><span data-ttu-id="d1169-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d1169-108">Properties</span></span>
|<span data-ttu-id="d1169-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d1169-109">Property</span></span>|<span data-ttu-id="d1169-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d1169-110">Type</span></span>|<span data-ttu-id="d1169-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d1169-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1169-112">описание</span><span class="sxs-lookup"><span data-stu-id="d1169-112">description</span></span>|<span data-ttu-id="d1169-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d1169-113">String</span></span>|<span data-ttu-id="d1169-114">Описание.</span><span class="sxs-lookup"><span data-stu-id="d1169-114">Description.</span></span>|
|<span data-ttu-id="d1169-115">address</span><span class="sxs-lookup"><span data-stu-id="d1169-115">address</span></span>|<span data-ttu-id="d1169-116">String</span><span class="sxs-lookup"><span data-stu-id="d1169-116">String</span></span>|<span data-ttu-id="d1169-117">Адрес (IP-адрес, URL-адрес или полное доменное имя)</span><span class="sxs-lookup"><span data-stu-id="d1169-117">Address (IP address, FQDN or URL)</span></span>|
|<span data-ttu-id="d1169-118">isDefaultServer</span><span class="sxs-lookup"><span data-stu-id="d1169-118">isDefaultServer</span></span>|<span data-ttu-id="d1169-119">Boolean.</span><span class="sxs-lookup"><span data-stu-id="d1169-119">Boolean</span></span>|<span data-ttu-id="d1169-120">Сервер по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="d1169-120">Default server.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1169-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d1169-121">Relationships</span></span>
<span data-ttu-id="d1169-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d1169-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1169-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d1169-123">JSON Representation</span></span>
<span data-ttu-id="d1169-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d1169-124">Here is a JSON representation of the resource.</span></span>
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





