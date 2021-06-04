---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0c561787c74649c6628768de691510524165f43f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52742736"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="3c6c3-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="3c6c3-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="3c6c3-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c6c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c6c3-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3c6c3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c6c3-106">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="3c6c3-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="3c6c3-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c6c3-107">Properties</span></span>
|<span data-ttu-id="3c6c3-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c6c3-108">Property</span></span>|<span data-ttu-id="3c6c3-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3c6c3-109">Type</span></span>|<span data-ttu-id="3c6c3-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3c6c3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c6c3-111">address</span><span class="sxs-lookup"><span data-stu-id="3c6c3-111">address</span></span>|<span data-ttu-id="3c6c3-112">String</span><span class="sxs-lookup"><span data-stu-id="3c6c3-112">String</span></span>|<span data-ttu-id="3c6c3-113">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="3c6c3-113">Address to the proxy server.</span></span> <span data-ttu-id="3c6c3-114">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="3c6c3-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="3c6c3-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="3c6c3-115">exceptions</span></span>|<span data-ttu-id="3c6c3-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3c6c3-116">String collection</span></span>|<span data-ttu-id="3c6c3-117">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="3c6c3-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="3c6c3-118">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="3c6c3-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="3c6c3-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="3c6c3-119">useForLocalAddresses</span></span>|<span data-ttu-id="3c6c3-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c6c3-120">Boolean</span></span>|<span data-ttu-id="3c6c3-121">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="3c6c3-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c6c3-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="3c6c3-122">Relationships</span></span>
<span data-ttu-id="3c6c3-123">Нет</span><span class="sxs-lookup"><span data-stu-id="3c6c3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3c6c3-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c6c3-124">JSON Representation</span></span>
<span data-ttu-id="3c6c3-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c6c3-125">Here is a JSON representation of the resource.</span></span>
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




