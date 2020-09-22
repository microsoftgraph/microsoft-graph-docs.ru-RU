---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 58fd5fb0e46b7458cf9c96c4f1b5d541ba60bf3b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091581"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="597f6-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="597f6-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="597f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="597f6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="597f6-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="597f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="597f6-106">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="597f6-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="597f6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="597f6-107">Properties</span></span>
|<span data-ttu-id="597f6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="597f6-108">Property</span></span>|<span data-ttu-id="597f6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="597f6-109">Type</span></span>|<span data-ttu-id="597f6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="597f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="597f6-111">address</span><span class="sxs-lookup"><span data-stu-id="597f6-111">address</span></span>|<span data-ttu-id="597f6-112">String</span><span class="sxs-lookup"><span data-stu-id="597f6-112">String</span></span>|<span data-ttu-id="597f6-113">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="597f6-113">Address to the proxy server.</span></span> <span data-ttu-id="597f6-114">Укажите адрес в формате \<server\> \[ :\<port\>\]</span><span class="sxs-lookup"><span data-stu-id="597f6-114">Specify an address in the format \<server\>\[:\<port\>\]</span></span>|
|<span data-ttu-id="597f6-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="597f6-115">exceptions</span></span>|<span data-ttu-id="597f6-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="597f6-116">String collection</span></span>|<span data-ttu-id="597f6-117">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="597f6-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="597f6-118">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="597f6-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="597f6-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="597f6-119">useForLocalAddresses</span></span>|<span data-ttu-id="597f6-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="597f6-120">Boolean</span></span>|<span data-ttu-id="597f6-121">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="597f6-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="597f6-122">Связи</span><span class="sxs-lookup"><span data-stu-id="597f6-122">Relationships</span></span>
<span data-ttu-id="597f6-123">Нет</span><span class="sxs-lookup"><span data-stu-id="597f6-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="597f6-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="597f6-124">JSON Representation</span></span>
<span data-ttu-id="597f6-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="597f6-125">Here is a JSON representation of the resource.</span></span>
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









