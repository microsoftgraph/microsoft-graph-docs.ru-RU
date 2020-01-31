---
title: Тип ресурса СпеЦифиедкаптивенетворкплугинс
description: Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d205218aab1ef6fb5a59280ff25f5a22fde8c0b
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636319"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="296ab-103">Тип ресурса СпеЦифиедкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="296ab-103">specifiedCaptiveNetworkPlugins resource type</span></span>

> <span data-ttu-id="296ab-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="296ab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="296ab-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="296ab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="296ab-106">Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="296ab-106">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="296ab-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="296ab-107">Properties</span></span>
|<span data-ttu-id="296ab-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="296ab-108">Property</span></span>|<span data-ttu-id="296ab-109">Тип</span><span class="sxs-lookup"><span data-stu-id="296ab-109">Type</span></span>|<span data-ttu-id="296ab-110">Описание</span><span class="sxs-lookup"><span data-stu-id="296ab-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="296ab-111">алловедбундлеидентифиерс</span><span class="sxs-lookup"><span data-stu-id="296ab-111">allowedBundleIdentifiers</span></span>|<span data-ttu-id="296ab-112">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="296ab-112">String collection</span></span>|<span data-ttu-id="296ab-113">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="296ab-113">Address of the IKEv2 server.</span></span> <span data-ttu-id="296ab-114">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="296ab-114">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="296ab-115">Связи</span><span class="sxs-lookup"><span data-stu-id="296ab-115">Relationships</span></span>
<span data-ttu-id="296ab-116">Нет</span><span class="sxs-lookup"><span data-stu-id="296ab-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="296ab-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="296ab-117">JSON Representation</span></span>
<span data-ttu-id="296ab-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="296ab-118">Here is a JSON representation of the resource.</span></span>
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



