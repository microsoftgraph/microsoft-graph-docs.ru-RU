---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 56c4b4bd526c69bf9992673aa8ae93d723a2d9bf
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456955"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="23d10-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="23d10-103">windows10NetworkProxyServer resource type</span></span>

<span data-ttu-id="23d10-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="23d10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="23d10-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="23d10-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23d10-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="23d10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23d10-107">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="23d10-107">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="23d10-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="23d10-108">Properties</span></span>
|<span data-ttu-id="23d10-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="23d10-109">Property</span></span>|<span data-ttu-id="23d10-110">Тип</span><span class="sxs-lookup"><span data-stu-id="23d10-110">Type</span></span>|<span data-ttu-id="23d10-111">Описание</span><span class="sxs-lookup"><span data-stu-id="23d10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23d10-112">address</span><span class="sxs-lookup"><span data-stu-id="23d10-112">address</span></span>|<span data-ttu-id="23d10-113">String</span><span class="sxs-lookup"><span data-stu-id="23d10-113">String</span></span>|<span data-ttu-id="23d10-114">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="23d10-114">Address to the proxy server.</span></span> <span data-ttu-id="23d10-115">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="23d10-115">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="23d10-116">exceptions</span><span class="sxs-lookup"><span data-stu-id="23d10-116">exceptions</span></span>|<span data-ttu-id="23d10-117">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="23d10-117">String collection</span></span>|<span data-ttu-id="23d10-118">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="23d10-118">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="23d10-119">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="23d10-119">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="23d10-120">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="23d10-120">useForLocalAddresses</span></span>|<span data-ttu-id="23d10-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="23d10-121">Boolean</span></span>|<span data-ttu-id="23d10-122">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="23d10-122">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23d10-123">Связи</span><span class="sxs-lookup"><span data-stu-id="23d10-123">Relationships</span></span>
<span data-ttu-id="23d10-124">Нет</span><span class="sxs-lookup"><span data-stu-id="23d10-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23d10-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="23d10-125">JSON Representation</span></span>
<span data-ttu-id="23d10-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="23d10-126">Here is a JSON representation of the resource.</span></span>
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



