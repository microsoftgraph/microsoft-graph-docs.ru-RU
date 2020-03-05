---
title: Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг
description: Автонастройка глобального прокси-сервера владельца устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 207cbafb423b322fd954d561a4204150cb078abf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42486600"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="274a5-103">Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг</span><span class="sxs-lookup"><span data-stu-id="274a5-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="274a5-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="274a5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="274a5-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="274a5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="274a5-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="274a5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="274a5-107">Автонастройка глобального прокси-сервера владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="274a5-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="274a5-108">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="274a5-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="274a5-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="274a5-109">Properties</span></span>
|<span data-ttu-id="274a5-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="274a5-110">Property</span></span>|<span data-ttu-id="274a5-111">Тип</span><span class="sxs-lookup"><span data-stu-id="274a5-111">Type</span></span>|<span data-ttu-id="274a5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="274a5-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="274a5-113">проксяутоконфигурл</span><span class="sxs-lookup"><span data-stu-id="274a5-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="274a5-114">String</span><span class="sxs-lookup"><span data-stu-id="274a5-114">String</span></span>|<span data-ttu-id="274a5-115">URL-адрес автоматической настройки прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="274a5-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="274a5-116">Связи</span><span class="sxs-lookup"><span data-stu-id="274a5-116">Relationships</span></span>
<span data-ttu-id="274a5-117">Нет</span><span class="sxs-lookup"><span data-stu-id="274a5-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="274a5-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="274a5-118">JSON Representation</span></span>
<span data-ttu-id="274a5-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="274a5-119">Here is a JSON representation of the resource.</span></span>
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



