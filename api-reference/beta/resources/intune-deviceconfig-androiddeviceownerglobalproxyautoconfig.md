---
title: Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг
description: Автонастройка глобального прокси-сервера владельца устройств Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86b00ccbe30568879a58bc1018d9c12fd36fa014
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708923"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="34f57-103">Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг</span><span class="sxs-lookup"><span data-stu-id="34f57-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="34f57-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34f57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34f57-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="34f57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34f57-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="34f57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34f57-107">Автонастройка глобального прокси-сервера владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="34f57-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="34f57-108">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="34f57-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="34f57-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="34f57-109">Properties</span></span>
|<span data-ttu-id="34f57-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="34f57-110">Property</span></span>|<span data-ttu-id="34f57-111">Тип</span><span class="sxs-lookup"><span data-stu-id="34f57-111">Type</span></span>|<span data-ttu-id="34f57-112">Описание</span><span class="sxs-lookup"><span data-stu-id="34f57-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34f57-113">проксяутоконфигурл</span><span class="sxs-lookup"><span data-stu-id="34f57-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="34f57-114">Строка</span><span class="sxs-lookup"><span data-stu-id="34f57-114">String</span></span>|<span data-ttu-id="34f57-115">URL-адрес автоматической настройки прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="34f57-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="34f57-116">Связи</span><span class="sxs-lookup"><span data-stu-id="34f57-116">Relationships</span></span>
<span data-ttu-id="34f57-117">Нет</span><span class="sxs-lookup"><span data-stu-id="34f57-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34f57-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="34f57-118">JSON Representation</span></span>
<span data-ttu-id="34f57-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="34f57-119">Here is a JSON representation of the resource.</span></span>
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





