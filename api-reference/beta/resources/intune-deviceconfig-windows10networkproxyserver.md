---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f2c8002423f394decbb2d52e9163581e4f254c92
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525644"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="732c6-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="732c6-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="732c6-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="732c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="732c6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="732c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="732c6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="732c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="732c6-107">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="732c6-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="732c6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="732c6-108">Properties</span></span>
|<span data-ttu-id="732c6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="732c6-109">Property</span></span>|<span data-ttu-id="732c6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="732c6-110">Type</span></span>|<span data-ttu-id="732c6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="732c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="732c6-112">address</span><span class="sxs-lookup"><span data-stu-id="732c6-112">address</span></span>|<span data-ttu-id="732c6-113">String</span><span class="sxs-lookup"><span data-stu-id="732c6-113">String</span></span>|<span data-ttu-id="732c6-114">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="732c6-114">Address to the proxy server.</span></span> <span data-ttu-id="732c6-115">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="732c6-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="732c6-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="732c6-116">exceptions</span></span>|<span data-ttu-id="732c6-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="732c6-117">String collection</span></span>|<span data-ttu-id="732c6-118">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="732c6-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="732c6-119">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="732c6-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="732c6-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="732c6-120">useForLocalAddresses</span></span>|<span data-ttu-id="732c6-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="732c6-121">Boolean</span></span>|<span data-ttu-id="732c6-122">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="732c6-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="732c6-123">Связи</span><span class="sxs-lookup"><span data-stu-id="732c6-123">Relationships</span></span>
<span data-ttu-id="732c6-124">Нет</span><span class="sxs-lookup"><span data-stu-id="732c6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="732c6-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="732c6-125">JSON Representation</span></span>
<span data-ttu-id="732c6-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="732c6-126">Here is a JSON representation of the resource.</span></span>
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



