---
title: Тип ресурса vpnProxyServer
description: VPN-сервер прокси-сервера.
ms.openlocfilehash: 31e711475bf0f797eead80ca3fe2f3c9af8ba27f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076172"
---
# <a name="vpnproxyserver-resource-type"></a><span data-ttu-id="19473-103">Тип ресурса vpnProxyServer</span><span class="sxs-lookup"><span data-stu-id="19473-103">vpnProxyServer resource type</span></span>

> <span data-ttu-id="19473-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="19473-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19473-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="19473-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19473-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="19473-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19473-107">VPN-сервер прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="19473-107">VPN Proxy Server.</span></span>
## <a name="properties"></a><span data-ttu-id="19473-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="19473-108">Properties</span></span>
|<span data-ttu-id="19473-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="19473-109">Property</span></span>|<span data-ttu-id="19473-110">Тип</span><span class="sxs-lookup"><span data-stu-id="19473-110">Type</span></span>|<span data-ttu-id="19473-111">Description</span><span class="sxs-lookup"><span data-stu-id="19473-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19473-112">automaticConfigurationScriptUrl</span><span class="sxs-lookup"><span data-stu-id="19473-112">automaticConfigurationScriptUrl</span></span>|<span data-ttu-id="19473-113">String</span><span class="sxs-lookup"><span data-stu-id="19473-113">String</span></span>|<span data-ttu-id="19473-114">Прокси-Автоматическая настройка сценария URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="19473-114">Proxy's automatic configuration script url.</span></span>|
|<span data-ttu-id="19473-115">address</span><span class="sxs-lookup"><span data-stu-id="19473-115">address</span></span>|<span data-ttu-id="19473-116">String</span><span class="sxs-lookup"><span data-stu-id="19473-116">String</span></span>|<span data-ttu-id="19473-117">Адрес.</span><span class="sxs-lookup"><span data-stu-id="19473-117">Address.</span></span>|
|<span data-ttu-id="19473-118">port</span><span class="sxs-lookup"><span data-stu-id="19473-118">port</span></span>|<span data-ttu-id="19473-119">Int32</span><span class="sxs-lookup"><span data-stu-id="19473-119">Int32</span></span>|<span data-ttu-id="19473-120">Порт.</span><span class="sxs-lookup"><span data-stu-id="19473-120">Port.</span></span> <span data-ttu-id="19473-121">Допустимые значения от 0 до 65535</span><span class="sxs-lookup"><span data-stu-id="19473-121">Valid values 0 to 65535</span></span>|

## <a name="relationships"></a><span data-ttu-id="19473-122">Связи</span><span class="sxs-lookup"><span data-stu-id="19473-122">Relationships</span></span>
<span data-ttu-id="19473-123">Нет</span><span class="sxs-lookup"><span data-stu-id="19473-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19473-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="19473-124">JSON Representation</span></span>
<span data-ttu-id="19473-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="19473-125">Here is a JSON representation of the resource.</span></span>
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





