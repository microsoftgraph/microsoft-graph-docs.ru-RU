---
title: Тип ресурса vpnProxyServer
description: VPN-сервер прокси-сервера.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 727d26af7f2c1801cd06fc98949109efec267f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27955354"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="c8a50-103">Тип ресурса vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="c8a50-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="c8a50-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c8a50-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c8a50-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c8a50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c8a50-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="c8a50-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8a50-107">VPN-сервер прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="c8a50-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="c8a50-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c8a50-108">Properties</span></span>
|<span data-ttu-id="c8a50-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c8a50-109">Property</span></span>|<span data-ttu-id="c8a50-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c8a50-110">Type</span></span>|<span data-ttu-id="c8a50-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c8a50-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8a50-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="c8a50-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="c8a50-113">Строка</span><span class="sxs-lookup"><span data-stu-id="c8a50-113">String</span></span>|<span data-ttu-id="c8a50-114">Прокси-Автоматическая настройка сценария URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="c8a50-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="c8a50-115">address</span><span class="sxs-lookup"><span data-stu-id="c8a50-115">address</span></span>|<span data-ttu-id="c8a50-116">String</span><span class="sxs-lookup"><span data-stu-id="c8a50-116">String</span></span>|<span data-ttu-id="c8a50-117">Адрес.</span><span class="sxs-lookup"><span data-stu-id="c8a50-117">Address.</span></span>|
|<span data-ttu-id="c8a50-118">port</span><span class="sxs-lookup"><span data-stu-id="c8a50-118">port</span></span>|<span data-ttu-id="c8a50-119">Int32</span><span class="sxs-lookup"><span data-stu-id="c8a50-119">Int32</span></span>|<span data-ttu-id="c8a50-120">Порт.</span><span class="sxs-lookup"><span data-stu-id="c8a50-120">Port.</span></span> <span data-ttu-id="c8a50-121">Допустимые значения от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="c8a50-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8a50-122">Связи</span><span class="sxs-lookup"><span data-stu-id="c8a50-122">Relationships</span></span>
<span data-ttu-id="c8a50-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c8a50-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8a50-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c8a50-124">JSON Representation</span></span>
<span data-ttu-id="c8a50-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c8a50-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnProxyServer",
  "automaticConfigurationScriptUrl": "String",
  "address": "String",
  "port": 1024
}
```





