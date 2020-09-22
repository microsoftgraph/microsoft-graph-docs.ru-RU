---
title: Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг
description: Автонастройка глобального прокси-сервера владельца устройств Android.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d6bbc652d3191d7129a0c44546e2360ccabbf0c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48085173"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="daf09-103">Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг</span><span class="sxs-lookup"><span data-stu-id="daf09-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

<span data-ttu-id="daf09-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="daf09-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="daf09-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="daf09-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="daf09-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="daf09-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="daf09-107">Автонастройка глобального прокси-сервера владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="daf09-107">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="daf09-108">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="daf09-108">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="daf09-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="daf09-109">Properties</span></span>
|<span data-ttu-id="daf09-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="daf09-110">Property</span></span>|<span data-ttu-id="daf09-111">Тип</span><span class="sxs-lookup"><span data-stu-id="daf09-111">Type</span></span>|<span data-ttu-id="daf09-112">Описание</span><span class="sxs-lookup"><span data-stu-id="daf09-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="daf09-113">проксяутоконфигурл</span><span class="sxs-lookup"><span data-stu-id="daf09-113">proxyAutoConfigURL</span></span>|<span data-ttu-id="daf09-114">Строка</span><span class="sxs-lookup"><span data-stu-id="daf09-114">String</span></span>|<span data-ttu-id="daf09-115">URL-адрес автоматической настройки прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="daf09-115">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="daf09-116">Связи</span><span class="sxs-lookup"><span data-stu-id="daf09-116">Relationships</span></span>
<span data-ttu-id="daf09-117">Нет</span><span class="sxs-lookup"><span data-stu-id="daf09-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="daf09-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="daf09-118">JSON Representation</span></span>
<span data-ttu-id="daf09-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="daf09-119">Here is a JSON representation of the resource.</span></span>
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






