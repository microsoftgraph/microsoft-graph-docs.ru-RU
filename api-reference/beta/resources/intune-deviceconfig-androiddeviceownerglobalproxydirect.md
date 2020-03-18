---
title: Тип ресурса Андроиддевицеовнерглобалпроксидирект
description: Глобальный прокси-сервер владельца устройств Android Direct.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cc2b960b85fd7fac506423af4d3a380247fb4892
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42797009"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="3afc2-103">Тип ресурса Андроиддевицеовнерглобалпроксидирект</span><span class="sxs-lookup"><span data-stu-id="3afc2-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

> <span data-ttu-id="3afc2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3afc2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3afc2-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3afc2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3afc2-106">Глобальный прокси-сервер владельца устройств Android Direct.</span><span class="sxs-lookup"><span data-stu-id="3afc2-106">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="3afc2-107">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="3afc2-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3afc2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3afc2-108">Properties</span></span>
|<span data-ttu-id="3afc2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3afc2-109">Property</span></span>|<span data-ttu-id="3afc2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3afc2-110">Type</span></span>|<span data-ttu-id="3afc2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3afc2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3afc2-112">host</span><span class="sxs-lookup"><span data-stu-id="3afc2-112">host</span></span>|<span data-ttu-id="3afc2-113">String</span><span class="sxs-lookup"><span data-stu-id="3afc2-113">String</span></span>|<span data-ttu-id="3afc2-114">Имя узла</span><span class="sxs-lookup"><span data-stu-id="3afc2-114">The host name</span></span>|
|<span data-ttu-id="3afc2-115">порта</span><span class="sxs-lookup"><span data-stu-id="3afc2-115">port</span></span>|<span data-ttu-id="3afc2-116">Int32</span><span class="sxs-lookup"><span data-stu-id="3afc2-116">Int32</span></span>|<span data-ttu-id="3afc2-117">Порт</span><span class="sxs-lookup"><span data-stu-id="3afc2-117">The port</span></span>|
|<span data-ttu-id="3afc2-118">ексклудедхостс</span><span class="sxs-lookup"><span data-stu-id="3afc2-118">excludedHosts</span></span>|<span data-ttu-id="3afc2-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3afc2-119">String collection</span></span>|<span data-ttu-id="3afc2-120">Исключенные узлы</span><span class="sxs-lookup"><span data-stu-id="3afc2-120">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="3afc2-121">Связи</span><span class="sxs-lookup"><span data-stu-id="3afc2-121">Relationships</span></span>
<span data-ttu-id="3afc2-122">Нет</span><span class="sxs-lookup"><span data-stu-id="3afc2-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3afc2-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3afc2-123">JSON Representation</span></span>
<span data-ttu-id="3afc2-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3afc2-124">Here is a JSON representation of the resource.</span></span>
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



