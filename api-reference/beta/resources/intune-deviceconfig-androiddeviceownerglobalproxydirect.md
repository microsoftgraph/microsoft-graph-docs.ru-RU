---
title: Тип ресурса Андроиддевицеовнерглобалпроксидирект
description: Глобальный прокси-сервер владельца устройств Android Direct.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cbe4329aacdfb151e0bb5b73f8b24b624010c327
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538646"
---
# <a name="androiddeviceownerglobalproxydirect-resource-type"></a><span data-ttu-id="0a4c4-103">Тип ресурса Андроиддевицеовнерглобалпроксидирект</span><span class="sxs-lookup"><span data-stu-id="0a4c4-103">androidDeviceOwnerGlobalProxyDirect resource type</span></span>

> <span data-ttu-id="0a4c4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0a4c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0a4c4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0a4c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a4c4-106">Глобальный прокси-сервер владельца устройств Android Direct.</span><span class="sxs-lookup"><span data-stu-id="0a4c4-106">Android Device Owner Global Proxy Direct.</span></span>


<span data-ttu-id="0a4c4-107">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="0a4c4-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0a4c4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="0a4c4-108">Properties</span></span>
|<span data-ttu-id="0a4c4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="0a4c4-109">Property</span></span>|<span data-ttu-id="0a4c4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="0a4c4-110">Type</span></span>|<span data-ttu-id="0a4c4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0a4c4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a4c4-112">host</span><span class="sxs-lookup"><span data-stu-id="0a4c4-112">host</span></span>|<span data-ttu-id="0a4c4-113">String</span><span class="sxs-lookup"><span data-stu-id="0a4c4-113">String</span></span>|<span data-ttu-id="0a4c4-114">Имя узла</span><span class="sxs-lookup"><span data-stu-id="0a4c4-114">The host name</span></span>|
|<span data-ttu-id="0a4c4-115">порта</span><span class="sxs-lookup"><span data-stu-id="0a4c4-115">port</span></span>|<span data-ttu-id="0a4c4-116">Int32</span><span class="sxs-lookup"><span data-stu-id="0a4c4-116">Int32</span></span>|<span data-ttu-id="0a4c4-117">Порт</span><span class="sxs-lookup"><span data-stu-id="0a4c4-117">The port</span></span>|
|<span data-ttu-id="0a4c4-118">ексклудедхостс</span><span class="sxs-lookup"><span data-stu-id="0a4c4-118">excludedHosts</span></span>|<span data-ttu-id="0a4c4-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="0a4c4-119">String collection</span></span>|<span data-ttu-id="0a4c4-120">Исключенные узлы</span><span class="sxs-lookup"><span data-stu-id="0a4c4-120">The excluded hosts</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a4c4-121">Связи</span><span class="sxs-lookup"><span data-stu-id="0a4c4-121">Relationships</span></span>
<span data-ttu-id="0a4c4-122">Нет</span><span class="sxs-lookup"><span data-stu-id="0a4c4-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0a4c4-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0a4c4-123">JSON Representation</span></span>
<span data-ttu-id="0a4c4-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0a4c4-124">Here is a JSON representation of the resource.</span></span>
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



