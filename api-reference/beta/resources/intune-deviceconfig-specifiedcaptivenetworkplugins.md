---
title: Тип ресурса СпеЦифиедкаптивенетворкплугинс
description: Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 30acdd502e13d2cf4ad1e5167978d1e675e2664a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787490"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="e741c-103">Тип ресурса СпеЦифиедкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="e741c-103">specifiedCaptiveNetworkPlugins resource type</span></span>

> <span data-ttu-id="e741c-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e741c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e741c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e741c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e741c-106">Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="e741c-106">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="e741c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e741c-107">Properties</span></span>
|<span data-ttu-id="e741c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e741c-108">Property</span></span>|<span data-ttu-id="e741c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e741c-109">Type</span></span>|<span data-ttu-id="e741c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e741c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e741c-111">алловедбундлеидентифиерс</span><span class="sxs-lookup"><span data-stu-id="e741c-111">allowedBundleIdentifiers</span></span>|<span data-ttu-id="e741c-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e741c-112">String collection</span></span>|<span data-ttu-id="e741c-113">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="e741c-113">Address of the IKEv2 server.</span></span> <span data-ttu-id="e741c-114">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="e741c-114">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="e741c-115">Связи</span><span class="sxs-lookup"><span data-stu-id="e741c-115">Relationships</span></span>
<span data-ttu-id="e741c-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e741c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e741c-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e741c-117">JSON Representation</span></span>
<span data-ttu-id="e741c-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e741c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.specifiedCaptiveNetworkPlugins",
  "allowedBundleIdentifiers": [
    "String"
  ]
}
```



