---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1dfe20e52ad63cf1d0d6a958f2ef5f4f89a53ad6
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30260699"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="357a3-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="357a3-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="357a3-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="357a3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="357a3-105">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="357a3-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="357a3-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="357a3-106">Properties</span></span>
|<span data-ttu-id="357a3-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="357a3-107">Property</span></span>|<span data-ttu-id="357a3-108">Тип</span><span class="sxs-lookup"><span data-stu-id="357a3-108">Type</span></span>|<span data-ttu-id="357a3-109">Описание</span><span class="sxs-lookup"><span data-stu-id="357a3-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="357a3-110">address</span><span class="sxs-lookup"><span data-stu-id="357a3-110">address</span></span>|<span data-ttu-id="357a3-111">String</span><span class="sxs-lookup"><span data-stu-id="357a3-111">String</span></span>|<span data-ttu-id="357a3-112">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="357a3-112">Address to the proxy server.</span></span> <span data-ttu-id="357a3-113">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="357a3-113">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="357a3-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="357a3-114">exceptions</span></span>|<span data-ttu-id="357a3-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="357a3-115">String collection</span></span>|<span data-ttu-id="357a3-116">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="357a3-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="357a3-117">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="357a3-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="357a3-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="357a3-118">useForLocalAddresses</span></span>|<span data-ttu-id="357a3-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="357a3-119">Boolean</span></span>|<span data-ttu-id="357a3-120">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="357a3-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="357a3-121">Связи</span><span class="sxs-lookup"><span data-stu-id="357a3-121">Relationships</span></span>
<span data-ttu-id="357a3-122">Нет</span><span class="sxs-lookup"><span data-stu-id="357a3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="357a3-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="357a3-123">JSON Representation</span></span>
<span data-ttu-id="357a3-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="357a3-124">Here is a JSON representation of the resource.</span></span>
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



