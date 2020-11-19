---
title: Тип ресурса Андроиддевицеовнерглобалпроксидирект
description: Глобальный прокси-сервер владельца устройств Android Direct.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dcbeac4a53a2cf07be562213f6202b7caa46f390
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303512"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="8d3ab-103">Тип ресурса Андроиддевицеовнерглобалпроксидирект</span><span class="sxs-lookup"><span data-stu-id="8d3ab-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

<span data-ttu-id="8d3ab-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8d3ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8d3ab-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8d3ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d3ab-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8d3ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d3ab-107">Глобальный прокси-сервер владельца устройств Android Direct.</span><span class="sxs-lookup"><span data-stu-id="8d3ab-107">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="8d3ab-108">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="8d3ab-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="8d3ab-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="8d3ab-109">Properties</span></span>
|<span data-ttu-id="8d3ab-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="8d3ab-110">Property</span></span>|<span data-ttu-id="8d3ab-111">Тип</span><span class="sxs-lookup"><span data-stu-id="8d3ab-111">Type</span></span>|<span data-ttu-id="8d3ab-112">Описание</span><span class="sxs-lookup"><span data-stu-id="8d3ab-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d3ab-113">host</span><span class="sxs-lookup"><span data-stu-id="8d3ab-113">host</span></span>|<span data-ttu-id="8d3ab-114">String</span><span class="sxs-lookup"><span data-stu-id="8d3ab-114">String</span></span>|<span data-ttu-id="8d3ab-115">Имя узла</span><span class="sxs-lookup"><span data-stu-id="8d3ab-115">The host name</span></span>|
|<span data-ttu-id="8d3ab-116">порта</span><span class="sxs-lookup"><span data-stu-id="8d3ab-116">port</span></span>|<span data-ttu-id="8d3ab-117">Int32</span><span class="sxs-lookup"><span data-stu-id="8d3ab-117">Int32</span></span>|<span data-ttu-id="8d3ab-118">Порт</span><span class="sxs-lookup"><span data-stu-id="8d3ab-118">The port</span></span>|
|<span data-ttu-id="8d3ab-119">ексклудедхостс</span><span class="sxs-lookup"><span data-stu-id="8d3ab-119">excludedHosts</span></span>|<span data-ttu-id="8d3ab-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="8d3ab-120">String collection</span></span>|<span data-ttu-id="8d3ab-121">Исключенные узлы</span><span class="sxs-lookup"><span data-stu-id="8d3ab-121">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="8d3ab-122">Связи</span><span class="sxs-lookup"><span data-stu-id="8d3ab-122">Relationships</span></span>
<span data-ttu-id="8d3ab-123">Нет</span><span class="sxs-lookup"><span data-stu-id="8d3ab-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d3ab-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8d3ab-124">JSON Representation</span></span>
<span data-ttu-id="8d3ab-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8d3ab-125">Here is a JSON representation of the resource.</span></span>
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




