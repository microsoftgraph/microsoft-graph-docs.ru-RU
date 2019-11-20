---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 88cf36813a6ed7102807917caf0bca3e46744f5f
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748464"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="ea566-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="ea566-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="ea566-104">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ea566-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea566-105">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="ea566-105">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="ea566-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea566-106">Properties</span></span>
|<span data-ttu-id="ea566-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea566-107">Property</span></span>|<span data-ttu-id="ea566-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ea566-108">Type</span></span>|<span data-ttu-id="ea566-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ea566-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea566-110">address</span><span class="sxs-lookup"><span data-stu-id="ea566-110">address</span></span>|<span data-ttu-id="ea566-111">String</span><span class="sxs-lookup"><span data-stu-id="ea566-111">String</span></span>|<span data-ttu-id="ea566-112">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="ea566-112">Address to the proxy server.</span></span> <span data-ttu-id="ea566-113">Укажите адрес в поле "сервер \<\>\[формата:\<порт".\>\]</span><span class="sxs-lookup"><span data-stu-id="ea566-113">Specify an address in the format \<server\>\[:\<port\>\]</span></span>|
|<span data-ttu-id="ea566-114">exceptions</span><span class="sxs-lookup"><span data-stu-id="ea566-114">exceptions</span></span>|<span data-ttu-id="ea566-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea566-115">String collection</span></span>|<span data-ttu-id="ea566-116">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="ea566-116">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="ea566-117">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="ea566-117">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="ea566-118">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="ea566-118">useForLocalAddresses</span></span>|<span data-ttu-id="ea566-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ea566-119">Boolean</span></span>|<span data-ttu-id="ea566-120">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="ea566-120">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea566-121">Связи</span><span class="sxs-lookup"><span data-stu-id="ea566-121">Relationships</span></span>
<span data-ttu-id="ea566-122">Нет</span><span class="sxs-lookup"><span data-stu-id="ea566-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea566-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea566-123">JSON Representation</span></span>
<span data-ttu-id="ea566-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea566-124">Here is a JSON representation of the resource.</span></span>
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




