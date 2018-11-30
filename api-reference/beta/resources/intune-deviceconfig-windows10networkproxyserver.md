---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
ms.openlocfilehash: 4e2e995c8d66249e5c742343f74e18e87337bfaa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080325"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="fb75d-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="fb75d-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="fb75d-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="fb75d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fb75d-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fb75d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fb75d-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="fb75d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fb75d-107">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="fb75d-107">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="fb75d-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fb75d-108">Properties</span></span>
|<span data-ttu-id="fb75d-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fb75d-109">Property</span></span>|<span data-ttu-id="fb75d-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fb75d-110">Type</span></span>|<span data-ttu-id="fb75d-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fb75d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb75d-112">address</span><span class="sxs-lookup"><span data-stu-id="fb75d-112">address</span></span>|<span data-ttu-id="fb75d-113">String</span><span class="sxs-lookup"><span data-stu-id="fb75d-113">String</span></span>|<span data-ttu-id="fb75d-114">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="fb75d-114">Address to the proxy server.</span></span> <span data-ttu-id="fb75d-115">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="fb75d-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="fb75d-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="fb75d-116">exceptions</span></span>|<span data-ttu-id="fb75d-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fb75d-117">String collection</span></span>|<span data-ttu-id="fb75d-118">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="fb75d-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="fb75d-119">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="fb75d-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="fb75d-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="fb75d-120">useForLocalAddresses</span></span>|<span data-ttu-id="fb75d-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="fb75d-121">Boolean</span></span>|<span data-ttu-id="fb75d-122">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="fb75d-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fb75d-123">Связи</span><span class="sxs-lookup"><span data-stu-id="fb75d-123">Relationships</span></span>
<span data-ttu-id="fb75d-124">Нет</span><span class="sxs-lookup"><span data-stu-id="fb75d-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="fb75d-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fb75d-125">JSON Representation</span></span>
<span data-ttu-id="fb75d-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fb75d-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```





