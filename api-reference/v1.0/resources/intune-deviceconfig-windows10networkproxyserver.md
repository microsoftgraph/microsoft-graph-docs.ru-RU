---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8b656805249e8406fbf2daa39612b168410b172e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530398"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="864a7-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="864a7-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="864a7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="864a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="864a7-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="864a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="864a7-106">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="864a7-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="864a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="864a7-107">Properties</span></span>
|<span data-ttu-id="864a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="864a7-108">Property</span></span>|<span data-ttu-id="864a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="864a7-109">Type</span></span>|<span data-ttu-id="864a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="864a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="864a7-111">address</span><span class="sxs-lookup"><span data-stu-id="864a7-111">address</span></span>|<span data-ttu-id="864a7-112">String</span><span class="sxs-lookup"><span data-stu-id="864a7-112">String</span></span>|<span data-ttu-id="864a7-113">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="864a7-113">Address to the proxy server.</span></span> <span data-ttu-id="864a7-114">Укажите адрес в поле "сервер \<\>\[формата:\<порт".\>\]</span><span class="sxs-lookup"><span data-stu-id="864a7-114">Specify an address in the format \<server\>\[:\<port\>\]</span></span>|
|<span data-ttu-id="864a7-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="864a7-115">exceptions</span></span>|<span data-ttu-id="864a7-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="864a7-116">String collection</span></span>|<span data-ttu-id="864a7-117">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="864a7-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="864a7-118">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="864a7-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="864a7-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="864a7-119">useForLocalAddresses</span></span>|<span data-ttu-id="864a7-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="864a7-120">Boolean</span></span>|<span data-ttu-id="864a7-121">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="864a7-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="864a7-122">Связи</span><span class="sxs-lookup"><span data-stu-id="864a7-122">Relationships</span></span>
<span data-ttu-id="864a7-123">Нет</span><span class="sxs-lookup"><span data-stu-id="864a7-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="864a7-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="864a7-124">JSON Representation</span></span>
<span data-ttu-id="864a7-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="864a7-125">Here is a JSON representation of the resource.</span></span>
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




