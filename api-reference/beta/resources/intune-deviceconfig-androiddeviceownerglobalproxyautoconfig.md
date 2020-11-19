---
title: Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг
description: Автонастройка глобального прокси-сервера владельца устройств Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 70b2fc59c2136364af0f2023b17c9f888fad8b6d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49303540"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="efba1-103">Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг</span><span class="sxs-lookup"><span data-stu-id="efba1-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="efba1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efba1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="efba1-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="efba1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="efba1-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="efba1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="efba1-107">Автонастройка глобального прокси-сервера владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="efba1-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="efba1-108">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="efba1-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="efba1-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="efba1-109">Properties</span></span>
|<span data-ttu-id="efba1-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="efba1-110">Property</span></span>|<span data-ttu-id="efba1-111">Тип</span><span class="sxs-lookup"><span data-stu-id="efba1-111">Type</span></span>|<span data-ttu-id="efba1-112">Описание</span><span class="sxs-lookup"><span data-stu-id="efba1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efba1-113">проксяутоконфигурл</span><span class="sxs-lookup"><span data-stu-id="efba1-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="efba1-114">String</span><span class="sxs-lookup"><span data-stu-id="efba1-114">String</span></span>|<span data-ttu-id="efba1-115">URL-адрес автоматической настройки прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="efba1-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="efba1-116">Связи</span><span class="sxs-lookup"><span data-stu-id="efba1-116">Relationships</span></span>
<span data-ttu-id="efba1-117">Нет</span><span class="sxs-lookup"><span data-stu-id="efba1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="efba1-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="efba1-118">JSON Representation</span></span>
<span data-ttu-id="efba1-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="efba1-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerGlobalProxyAutoConfig",
  "proxyAutoConfigURL": "String"
}
```




