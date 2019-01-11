---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 2dcdb371ddcf7887fee8169eb29bbd856e5b8ab2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806169"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="62a00-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="62a00-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="62a00-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="62a00-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62a00-105">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="62a00-105">Network Proxy Server Policy.</span></span>
## <a name="properties"></a><span data-ttu-id="62a00-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="62a00-106">Properties</span></span>
|<span data-ttu-id="62a00-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="62a00-107">Property</span></span>|<span data-ttu-id="62a00-108">Тип</span><span class="sxs-lookup"><span data-stu-id="62a00-108">Type</span></span>|<span data-ttu-id="62a00-109">Описание</span><span class="sxs-lookup"><span data-stu-id="62a00-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a00-110">address</span><span class="sxs-lookup"><span data-stu-id="62a00-110">address</span></span>|<span data-ttu-id="62a00-111">String</span><span class="sxs-lookup"><span data-stu-id="62a00-111">String</span></span>|<span data-ttu-id="62a00-112">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="62a00-112">Address to the proxy server.</span></span> <span data-ttu-id="62a00-113">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="62a00-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="62a00-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="62a00-114">exceptions</span></span>|<span data-ttu-id="62a00-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="62a00-115">String collection</span></span>|<span data-ttu-id="62a00-116">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="62a00-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="62a00-117">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="62a00-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="62a00-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="62a00-118">useForLocalAddresses</span></span>|<span data-ttu-id="62a00-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="62a00-119">Boolean</span></span>|<span data-ttu-id="62a00-120">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="62a00-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62a00-121">Связи</span><span class="sxs-lookup"><span data-stu-id="62a00-121">Relationships</span></span>
<span data-ttu-id="62a00-122">Нет</span><span class="sxs-lookup"><span data-stu-id="62a00-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="62a00-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="62a00-123">JSON Representation</span></span>
<span data-ttu-id="62a00-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="62a00-124">Here is a JSON representation of the resource.</span></span>
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



