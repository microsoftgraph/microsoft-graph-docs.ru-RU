---
title: Тип ресурса Андроиддевицеовнерглобалпроксидирект
description: Глобальный прокси-сервер владельца устройств Android Direct.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 58e95490fa3fd7adaec6e6b8f01c43566b1c289a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486551"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="70930-103">Тип ресурса Андроиддевицеовнерглобалпроксидирект</span><span class="sxs-lookup"><span data-stu-id="70930-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

<span data-ttu-id="70930-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="70930-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="70930-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="70930-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70930-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="70930-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70930-107">Глобальный прокси-сервер владельца устройств Android Direct.</span><span class="sxs-lookup"><span data-stu-id="70930-107">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="70930-108">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="70930-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="70930-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="70930-109">Properties</span></span>
|<span data-ttu-id="70930-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="70930-110">Property</span></span>|<span data-ttu-id="70930-111">Тип</span><span class="sxs-lookup"><span data-stu-id="70930-111">Type</span></span>|<span data-ttu-id="70930-112">Описание</span><span class="sxs-lookup"><span data-stu-id="70930-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70930-113">host</span><span class="sxs-lookup"><span data-stu-id="70930-113">host</span></span>|<span data-ttu-id="70930-114">String</span><span class="sxs-lookup"><span data-stu-id="70930-114">String</span></span>|<span data-ttu-id="70930-115">Имя узла</span><span class="sxs-lookup"><span data-stu-id="70930-115">The host name</span></span>|
|<span data-ttu-id="70930-116">порта</span><span class="sxs-lookup"><span data-stu-id="70930-116">port</span></span>|<span data-ttu-id="70930-117">Int32</span><span class="sxs-lookup"><span data-stu-id="70930-117">Int32</span></span>|<span data-ttu-id="70930-118">Порт</span><span class="sxs-lookup"><span data-stu-id="70930-118">The port</span></span>|
|<span data-ttu-id="70930-119">ексклудедхостс</span><span class="sxs-lookup"><span data-stu-id="70930-119">excludedHosts</span></span>|<span data-ttu-id="70930-120">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="70930-120">String collection</span></span>|<span data-ttu-id="70930-121">Исключенные узлы</span><span class="sxs-lookup"><span data-stu-id="70930-121">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="70930-122">Связи</span><span class="sxs-lookup"><span data-stu-id="70930-122">Relationships</span></span>
<span data-ttu-id="70930-123">Нет</span><span class="sxs-lookup"><span data-stu-id="70930-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="70930-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="70930-124">JSON Representation</span></span>
<span data-ttu-id="70930-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="70930-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyDirect"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyDirect",
  "host": "String",
  "port": 1024,
  "excludedHosts": [
    "String"
  ]
}
```



