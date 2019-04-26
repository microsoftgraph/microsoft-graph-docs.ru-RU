---
title: Тип ресурса windows10NetworkProxyServer
description: Политика прокси-сервера сети.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 120eff89a01434803c1e2f4f5ba84d3f088e1022
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571963"
---
# <a name="windows10networkproxyserver-resource-type"></a><span data-ttu-id="d428d-103">Тип ресурса windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="d428d-103">windows10NetworkProxyServer resource type</span></span>

> <span data-ttu-id="d428d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d428d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d428d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d428d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d428d-106">Политика прокси-сервера сети.</span><span class="sxs-lookup"><span data-stu-id="d428d-106">Network Proxy Server Policy.</span></span>

## <a name="properties"></a><span data-ttu-id="d428d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d428d-107">Properties</span></span>
|<span data-ttu-id="d428d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d428d-108">Property</span></span>|<span data-ttu-id="d428d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d428d-109">Type</span></span>|<span data-ttu-id="d428d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d428d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d428d-111">address</span><span class="sxs-lookup"><span data-stu-id="d428d-111">address</span></span>|<span data-ttu-id="d428d-112">String</span><span class="sxs-lookup"><span data-stu-id="d428d-112">String</span></span>|<span data-ttu-id="d428d-113">Адрес прокси-сервера.</span><span class="sxs-lookup"><span data-stu-id="d428d-113">Address to the proxy server.</span></span> <span data-ttu-id="d428d-114">Укажите адрес в формате <server>\[":"<port>\]</span><span class="sxs-lookup"><span data-stu-id="d428d-114">Specify an address in the format <server>\[“:”<port>\]</span></span>|
|<span data-ttu-id="d428d-115">exceptions</span><span class="sxs-lookup"><span data-stu-id="d428d-115">exceptions</span></span>|<span data-ttu-id="d428d-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d428d-116">String collection</span></span>|<span data-ttu-id="d428d-117">Адреса, которые не должны использовать прокси-сервер.</span><span class="sxs-lookup"><span data-stu-id="d428d-117">Addresses that should not use the proxy server.</span></span> <span data-ttu-id="d428d-118">Система не использует прокси-сервер для адресов, начинающихся, как указано в этом узле.</span><span class="sxs-lookup"><span data-stu-id="d428d-118">The system will not use the proxy server for addresses beginning with what is specified in this node.</span></span>|
|<span data-ttu-id="d428d-119">useForLocalAddresses</span><span class="sxs-lookup"><span data-stu-id="d428d-119">useForLocalAddresses</span></span>|<span data-ttu-id="d428d-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="d428d-120">Boolean</span></span>|<span data-ttu-id="d428d-121">Определяет необходимость использования прокси-сервера для локальных адресов (в интрасети).</span><span class="sxs-lookup"><span data-stu-id="d428d-121">Specifies whether the proxy server should be used for local (intranet) addresses.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d428d-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="d428d-122">Relationships</span></span>
<span data-ttu-id="d428d-123">Нет</span><span class="sxs-lookup"><span data-stu-id="d428d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d428d-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d428d-124">JSON Representation</span></span>
<span data-ttu-id="d428d-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d428d-125">Here is a JSON representation of the resource.</span></span>
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





