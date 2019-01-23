---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 673cfe99e9cafe1b57fde5c70b7059286a6cc554
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418584"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="bf387-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="bf387-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="bf387-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bf387-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bf387-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bf387-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bf387-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bf387-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf387-107">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="bf387-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="bf387-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bf387-108">Properties</span></span>
|<span data-ttu-id="bf387-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bf387-109">Property</span></span>|<span data-ttu-id="bf387-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bf387-110">Type</span></span>|<span data-ttu-id="bf387-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bf387-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf387-112">address</span><span class="sxs-lookup"><span data-stu-id="bf387-112">address</span></span>|<span data-ttu-id="bf387-113">String</span><span class="sxs-lookup"><span data-stu-id="bf387-113">String</span></span>|<span data-ttu-id="bf387-114">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="bf387-114">Address to the proxy server.</span></span> <span data-ttu-id="bf387-115">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="bf387-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="bf387-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="bf387-116">exceptions</span></span>|<span data-ttu-id="bf387-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="bf387-117">String collection</span></span>|<span data-ttu-id="bf387-118">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="bf387-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="bf387-119">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="bf387-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="bf387-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="bf387-120">useForLocalAddresses</span></span>|<span data-ttu-id="bf387-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="bf387-121">Boolean</span></span>|<span data-ttu-id="bf387-122">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="bf387-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf387-123">Связи</span><span class="sxs-lookup"><span data-stu-id="bf387-123">Relationships</span></span>
<span data-ttu-id="bf387-124">Нет</span><span class="sxs-lookup"><span data-stu-id="bf387-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf387-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bf387-125">JSON Representation</span></span>
<span data-ttu-id="bf387-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bf387-126">Here is a JSON representation of the resource.</span></span>
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




