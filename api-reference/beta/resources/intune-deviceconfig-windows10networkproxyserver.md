---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f02444a1cfccd2638f9fa6872b6b35dab649287
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786679"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="1ccf4-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="1ccf4-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="1ccf4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1ccf4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ccf4-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="1ccf4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ccf4-106">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="1ccf4-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="1ccf4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="1ccf4-107">Properties</span></span>
|<span data-ttu-id="1ccf4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="1ccf4-108">Property</span></span>|<span data-ttu-id="1ccf4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="1ccf4-109">Type</span></span>|<span data-ttu-id="1ccf4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1ccf4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ccf4-111">address</span><span class="sxs-lookup"><span data-stu-id="1ccf4-111">address</span></span>|<span data-ttu-id="1ccf4-112">String</span><span class="sxs-lookup"><span data-stu-id="1ccf4-112">String</span></span>|<span data-ttu-id="1ccf4-113">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="1ccf4-113">Address to the proxy server.</span></span> <span data-ttu-id="1ccf4-114">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="1ccf4-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="1ccf4-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="1ccf4-115">exceptions</span></span>|<span data-ttu-id="1ccf4-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="1ccf4-116">String collection</span></span>|<span data-ttu-id="1ccf4-117">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="1ccf4-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="1ccf4-118">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="1ccf4-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="1ccf4-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="1ccf4-119">useForLocalAddresses</span></span>|<span data-ttu-id="1ccf4-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ccf4-120">Boolean</span></span>|<span data-ttu-id="1ccf4-121">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="1ccf4-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1ccf4-122">Связи</span><span class="sxs-lookup"><span data-stu-id="1ccf4-122">Relationships</span></span>
<span data-ttu-id="1ccf4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="1ccf4-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ccf4-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1ccf4-124">JSON Representation</span></span>
<span data-ttu-id="1ccf4-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1ccf4-125">Here is a JSON representation of the resource.</span></span>
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



