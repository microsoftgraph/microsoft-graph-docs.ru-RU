---
title: Тип ресурса Иосвебконтентфилтераутофилтер
description: Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b3bcf8c66aff4220b7e2b394819beb35255bfba3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529821"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="fc468-104">Тип ресурса Иосвебконтентфилтераутофилтер</span><span class="sxs-lookup"><span data-stu-id="fc468-104">iosWebContentFilterAutoFilter resource type</span></span>

<span data-ttu-id="fc468-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="fc468-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc468-106">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="fc468-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc468-107">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="fc468-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc468-108">Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="fc468-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="fc468-109">При создании без значений свойств устройство iOS включит автоматический фильтр независимо.</span><span class="sxs-lookup"><span data-stu-id="fc468-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="fc468-110">Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="fc468-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="fc468-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="fc468-111">Properties</span></span>
|<span data-ttu-id="fc468-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="fc468-112">Property</span></span>|<span data-ttu-id="fc468-113">Тип</span><span class="sxs-lookup"><span data-stu-id="fc468-113">Type</span></span>|<span data-ttu-id="fc468-114">Описание</span><span class="sxs-lookup"><span data-stu-id="fc468-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc468-115">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="fc468-115">allowedUrls</span></span>|<span data-ttu-id="fc468-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc468-116">String collection</span></span>|<span data-ttu-id="fc468-117">Дополнительные URL-адреса, разрешенные для Access</span><span class="sxs-lookup"><span data-stu-id="fc468-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="fc468-118">блоккедурлс</span><span class="sxs-lookup"><span data-stu-id="fc468-118">blockedUrls</span></span>|<span data-ttu-id="fc468-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="fc468-119">String collection</span></span>|<span data-ttu-id="fc468-120">Дополнительные URL-адреса, заблокированные для Access</span><span class="sxs-lookup"><span data-stu-id="fc468-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc468-121">Связи</span><span class="sxs-lookup"><span data-stu-id="fc468-121">Relationships</span></span>
<span data-ttu-id="fc468-122">Нет</span><span class="sxs-lookup"><span data-stu-id="fc468-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc468-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="fc468-123">JSON Representation</span></span>
<span data-ttu-id="fc468-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fc468-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```



