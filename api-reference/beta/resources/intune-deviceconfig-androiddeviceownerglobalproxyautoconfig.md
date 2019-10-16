---
title: Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг
description: Автонастройка глобального прокси-сервера владельца устройств Android.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e15b3009537bd55eb7d4af6d93bbea3b53f3325a
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538653"
---
# <a name="androiddeviceownerglobalproxyautoconfig-resource-type"></a><span data-ttu-id="07dac-103">Тип ресурса Андроиддевицеовнерглобалпроксяутоконфиг</span><span class="sxs-lookup"><span data-stu-id="07dac-103">androidDeviceOwnerGlobalProxyAutoConfig resource type</span></span>

> <span data-ttu-id="07dac-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07dac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07dac-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07dac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07dac-106">Автонастройка глобального прокси-сервера владельца устройств Android.</span><span class="sxs-lookup"><span data-stu-id="07dac-106">Android Device Owner Global Proxy Auto Config.</span></span>


<span data-ttu-id="07dac-107">Наследуется от [андроиддевицеовнерглобалпрокси](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span><span class="sxs-lookup"><span data-stu-id="07dac-107">Inherits from [androidDeviceOwnerGlobalProxy](../resources/intune-deviceconfig-androiddeviceownerglobalproxy.md)</span></span>

## <a name="properties"></a><span data-ttu-id="07dac-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07dac-108">Properties</span></span>
|<span data-ttu-id="07dac-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="07dac-109">Property</span></span>|<span data-ttu-id="07dac-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07dac-110">Type</span></span>|<span data-ttu-id="07dac-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07dac-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07dac-112">проксяутоконфигурл</span><span class="sxs-lookup"><span data-stu-id="07dac-112">proxyAutoConfigURL</span></span>|<span data-ttu-id="07dac-113">String</span><span class="sxs-lookup"><span data-stu-id="07dac-113">String</span></span>|<span data-ttu-id="07dac-114">URL-адрес автоматической настройки прокси-сервера</span><span class="sxs-lookup"><span data-stu-id="07dac-114">The proxy auto-config URL</span></span>|

## <a name="relationships"></a><span data-ttu-id="07dac-115">Связи</span><span class="sxs-lookup"><span data-stu-id="07dac-115">Relationships</span></span>
<span data-ttu-id="07dac-116">Нет</span><span class="sxs-lookup"><span data-stu-id="07dac-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07dac-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07dac-117">JSON Representation</span></span>
<span data-ttu-id="07dac-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07dac-118">Here is a JSON representation of the resource.</span></span>
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



