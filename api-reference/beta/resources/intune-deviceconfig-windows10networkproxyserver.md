---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cc0ec2256d5205a5110651e6c2dce3f46f8c8465
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272824"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="ff2c1-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="ff2c1-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="ff2c1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff2c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff2c1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ff2c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff2c1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ff2c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff2c1-107">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="ff2c1-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="ff2c1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ff2c1-108">Properties</span></span>
|<span data-ttu-id="ff2c1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ff2c1-109">Property</span></span>|<span data-ttu-id="ff2c1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ff2c1-110">Type</span></span>|<span data-ttu-id="ff2c1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ff2c1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff2c1-112">address</span><span class="sxs-lookup"><span data-stu-id="ff2c1-112">address</span></span>|<span data-ttu-id="ff2c1-113">String</span><span class="sxs-lookup"><span data-stu-id="ff2c1-113">String</span></span>|<span data-ttu-id="ff2c1-114">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="ff2c1-114">Address to the proxy server.</span></span> <span data-ttu-id="ff2c1-115">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="ff2c1-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="ff2c1-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="ff2c1-116">exceptions</span></span>|<span data-ttu-id="ff2c1-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ff2c1-117">String collection</span></span>|<span data-ttu-id="ff2c1-118">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="ff2c1-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="ff2c1-119">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="ff2c1-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="ff2c1-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="ff2c1-120">useForLocalAddresses</span></span>|<span data-ttu-id="ff2c1-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="ff2c1-121">Boolean</span></span>|<span data-ttu-id="ff2c1-122">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="ff2c1-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff2c1-123">Связи</span><span class="sxs-lookup"><span data-stu-id="ff2c1-123">Relationships</span></span>
<span data-ttu-id="ff2c1-124">Нет</span><span class="sxs-lookup"><span data-stu-id="ff2c1-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff2c1-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ff2c1-125">JSON Representation</span></span>
<span data-ttu-id="ff2c1-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ff2c1-126">Here is a JSON representation of the resource.</span></span>
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




