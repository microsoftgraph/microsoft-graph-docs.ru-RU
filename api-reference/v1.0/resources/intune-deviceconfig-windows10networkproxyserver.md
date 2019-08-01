---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b68f13ab80544d591b22fc77ab35110302dc48ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031012"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="33e96-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="33e96-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="33e96-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="33e96-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33e96-105">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="33e96-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="33e96-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="33e96-106">Properties</span></span>
|<span data-ttu-id="33e96-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="33e96-107">Property</span></span>|<span data-ttu-id="33e96-108">Тип</span><span class="sxs-lookup"><span data-stu-id="33e96-108">Type</span></span>|<span data-ttu-id="33e96-109">Описание</span><span class="sxs-lookup"><span data-stu-id="33e96-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33e96-110">address</span><span class="sxs-lookup"><span data-stu-id="33e96-110">address</span></span>|<span data-ttu-id="33e96-111">String</span><span class="sxs-lookup"><span data-stu-id="33e96-111">String</span></span>|<span data-ttu-id="33e96-112">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="33e96-112">Address to the proxy server.</span></span> <span data-ttu-id="33e96-113">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="33e96-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="33e96-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="33e96-114">exceptions</span></span>|<span data-ttu-id="33e96-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="33e96-115">String collection</span></span>|<span data-ttu-id="33e96-116">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="33e96-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="33e96-117">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="33e96-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="33e96-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="33e96-118">useForLocalAddresses</span></span>|<span data-ttu-id="33e96-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="33e96-119">Boolean</span></span>|<span data-ttu-id="33e96-120">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="33e96-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33e96-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="33e96-121">Relationships</span></span>
<span data-ttu-id="33e96-122">Нет</span><span class="sxs-lookup"><span data-stu-id="33e96-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="33e96-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="33e96-123">JSON Representation</span></span>
<span data-ttu-id="33e96-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="33e96-124">Here is a JSON representation of the resource.</span></span>
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



