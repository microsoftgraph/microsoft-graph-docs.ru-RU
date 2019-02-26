---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f29c69789f6b2a4d41bbb5179ff71f721c64c88f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162106"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="91c57-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="91c57-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="91c57-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="91c57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91c57-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="91c57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91c57-106">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="91c57-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="91c57-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="91c57-107">Properties</span></span>
|<span data-ttu-id="91c57-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="91c57-108">Property</span></span>|<span data-ttu-id="91c57-109">Тип</span><span class="sxs-lookup"><span data-stu-id="91c57-109">Type</span></span>|<span data-ttu-id="91c57-110">Описание</span><span class="sxs-lookup"><span data-stu-id="91c57-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91c57-111">address</span><span class="sxs-lookup"><span data-stu-id="91c57-111">address</span></span>|<span data-ttu-id="91c57-112">String</span><span class="sxs-lookup"><span data-stu-id="91c57-112">String</span></span>|<span data-ttu-id="91c57-113">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="91c57-113">Address to the proxy server.</span></span> <span data-ttu-id="91c57-114">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="91c57-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="91c57-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="91c57-115">exceptions</span></span>|<span data-ttu-id="91c57-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="91c57-116">String collection</span></span>|<span data-ttu-id="91c57-117">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="91c57-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="91c57-118">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="91c57-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="91c57-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="91c57-119">useForLocalAddresses</span></span>|<span data-ttu-id="91c57-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="91c57-120">Boolean</span></span>|<span data-ttu-id="91c57-121">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="91c57-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="91c57-122">Связи</span><span class="sxs-lookup"><span data-stu-id="91c57-122">Relationships</span></span>
<span data-ttu-id="91c57-123">Нет</span><span class="sxs-lookup"><span data-stu-id="91c57-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="91c57-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="91c57-124">JSON Representation</span></span>
<span data-ttu-id="91c57-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="91c57-125">Here is a JSON representation of the resource.</span></span>
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




