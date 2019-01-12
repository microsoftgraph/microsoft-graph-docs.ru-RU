---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4e9f727916f055fe197f98b07625b00406e16e83
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27921103"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="a9749-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="a9749-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="a9749-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="a9749-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a9749-105">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="a9749-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="a9749-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a9749-106">Properties</span></span>
|<span data-ttu-id="a9749-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a9749-107">Property</span></span>|<span data-ttu-id="a9749-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a9749-108">Type</span></span>|<span data-ttu-id="a9749-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a9749-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9749-110">address</span><span class="sxs-lookup"><span data-stu-id="a9749-110">address</span></span>|<span data-ttu-id="a9749-111">String</span><span class="sxs-lookup"><span data-stu-id="a9749-111">String</span></span>|<span data-ttu-id="a9749-112">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="a9749-112">Address to the proxy server.</span></span> <span data-ttu-id="a9749-113">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="a9749-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="a9749-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="a9749-114">exceptions</span></span>|<span data-ttu-id="a9749-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a9749-115">String collection</span></span>|<span data-ttu-id="a9749-116">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="a9749-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="a9749-117">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="a9749-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="a9749-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="a9749-118">useForLocalAddresses</span></span>|<span data-ttu-id="a9749-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="a9749-119">Boolean</span></span>|<span data-ttu-id="a9749-120">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="a9749-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a9749-121">Связи</span><span class="sxs-lookup"><span data-stu-id="a9749-121">Relationships</span></span>
<span data-ttu-id="a9749-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a9749-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a9749-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a9749-123">JSON Representation</span></span>
<span data-ttu-id="a9749-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a9749-124">Here is a JSON representation of the resource.</span></span>
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



