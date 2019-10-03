---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b126358a8ab8574d4dcbf7c1f22e412eda41d61f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367058"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="78a3a-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="78a3a-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="78a3a-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="78a3a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78a3a-105">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="78a3a-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="78a3a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="78a3a-106">Properties</span></span>
|<span data-ttu-id="78a3a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="78a3a-107">Property</span></span>|<span data-ttu-id="78a3a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="78a3a-108">Type</span></span>|<span data-ttu-id="78a3a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="78a3a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78a3a-110">address</span><span class="sxs-lookup"><span data-stu-id="78a3a-110">address</span></span>|<span data-ttu-id="78a3a-111">String</span><span class="sxs-lookup"><span data-stu-id="78a3a-111">String</span></span>|<span data-ttu-id="78a3a-112">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="78a3a-112">Address to the proxy server.</span></span> <span data-ttu-id="78a3a-113">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="78a3a-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="78a3a-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="78a3a-114">exceptions</span></span>|<span data-ttu-id="78a3a-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="78a3a-115">String collection</span></span>|<span data-ttu-id="78a3a-116">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="78a3a-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="78a3a-117">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="78a3a-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="78a3a-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="78a3a-118">useForLocalAddresses</span></span>|<span data-ttu-id="78a3a-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="78a3a-119">Boolean</span></span>|<span data-ttu-id="78a3a-120">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="78a3a-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="78a3a-121">Связи</span><span class="sxs-lookup"><span data-stu-id="78a3a-121">Relationships</span></span>
<span data-ttu-id="78a3a-122">Нет</span><span class="sxs-lookup"><span data-stu-id="78a3a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78a3a-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="78a3a-123">JSON Representation</span></span>
<span data-ttu-id="78a3a-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="78a3a-124">Here is a JSON representation of the resource.</span></span>
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




