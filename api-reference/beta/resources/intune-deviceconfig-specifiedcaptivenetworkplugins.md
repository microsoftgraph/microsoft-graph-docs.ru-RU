---
title: Тип ресурса СпеЦифиедкаптивенетворкплугинс
description: Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6752e045817e9a03eefae178d7df15d152f0ea58
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412771"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a><span data-ttu-id="fc16e-103">Тип ресурса СпеЦифиедкаптивенетворкплугинс</span><span class="sxs-lookup"><span data-stu-id="fc16e-103">specifiedCaptiveNetworkPlugins resource type</span></span>

<span data-ttu-id="fc16e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc16e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc16e-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc16e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc16e-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc16e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc16e-107">Задает все сетевые подключаемые модули, разрешенные во время VPN-подключения IKEv2 AlwaysOn.</span><span class="sxs-lookup"><span data-stu-id="fc16e-107">Specifies all the Captive network plugins allowed during the IKEv2 AlwaysOn VPN connection</span></span>

## <a name="properties"></a><span data-ttu-id="fc16e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc16e-108">Properties</span></span>
|<span data-ttu-id="fc16e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc16e-109">Property</span></span>|<span data-ttu-id="fc16e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="fc16e-110">Type</span></span>|<span data-ttu-id="fc16e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="fc16e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc16e-112">алловедбундлеидентифиерс</span><span class="sxs-lookup"><span data-stu-id="fc16e-112">allowedBundleIdentifiers</span></span>|<span data-ttu-id="fc16e-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc16e-113">String collection</span></span>|<span data-ttu-id="fc16e-114">Адрес сервера IKEv2.</span><span class="sxs-lookup"><span data-stu-id="fc16e-114">Address of the IKEv2 server.</span></span> <span data-ttu-id="fc16e-115">Должно быть полным доменным именем, Усерфкдн, сетевым адресом или ASN1DN</span><span class="sxs-lookup"><span data-stu-id="fc16e-115">Must be a FQDN, UserFQDN, network address, or ASN1DN</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc16e-116">Связи</span><span class="sxs-lookup"><span data-stu-id="fc16e-116">Relationships</span></span>
<span data-ttu-id="fc16e-117">Нет</span><span class="sxs-lookup"><span data-stu-id="fc16e-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc16e-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc16e-118">JSON Representation</span></span>
<span data-ttu-id="fc16e-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc16e-119">Here is a JSON representation of the resource.</span></span>
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



