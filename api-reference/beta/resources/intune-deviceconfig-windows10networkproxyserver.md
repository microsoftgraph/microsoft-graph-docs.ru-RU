---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 59290b2f31657e5f75aba1fe804a625d82d4c7b0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000363"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="95b18-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="95b18-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="95b18-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="95b18-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95b18-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="95b18-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95b18-106">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="95b18-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="95b18-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="95b18-107">Properties</span></span>
|<span data-ttu-id="95b18-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="95b18-108">Property</span></span>|<span data-ttu-id="95b18-109">Тип</span><span class="sxs-lookup"><span data-stu-id="95b18-109">Type</span></span>|<span data-ttu-id="95b18-110">Описание</span><span class="sxs-lookup"><span data-stu-id="95b18-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95b18-111">address</span><span class="sxs-lookup"><span data-stu-id="95b18-111">address</span></span>|<span data-ttu-id="95b18-112">String</span><span class="sxs-lookup"><span data-stu-id="95b18-112">String</span></span>|<span data-ttu-id="95b18-113">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="95b18-113">Address to the proxy server.</span></span> <span data-ttu-id="95b18-114">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="95b18-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="95b18-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="95b18-115">exceptions</span></span>|<span data-ttu-id="95b18-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="95b18-116">String collection</span></span>|<span data-ttu-id="95b18-117">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="95b18-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="95b18-118">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="95b18-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="95b18-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="95b18-119">useForLocalAddresses</span></span>|<span data-ttu-id="95b18-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="95b18-120">Boolean</span></span>|<span data-ttu-id="95b18-121">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="95b18-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="95b18-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="95b18-122">Relationships</span></span>
<span data-ttu-id="95b18-123">Нет</span><span class="sxs-lookup"><span data-stu-id="95b18-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="95b18-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="95b18-124">JSON Representation</span></span>
<span data-ttu-id="95b18-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="95b18-125">Here is a JSON representation of the resource.</span></span>
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





