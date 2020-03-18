---
title: Тип ресурса Иосвебконтентфилтераутофилтер
description: Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 61054fa3e8d8894203a72b32cbb68ebb91e05aeb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42790477"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="90ba6-104">Тип ресурса Иосвебконтентфилтераутофилтер</span><span class="sxs-lookup"><span data-stu-id="90ba6-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="90ba6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="90ba6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90ba6-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="90ba6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90ba6-107">Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="90ba6-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="90ba6-108">При создании без значений свойств устройство iOS включит автоматический фильтр независимо.</span><span class="sxs-lookup"><span data-stu-id="90ba6-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="90ba6-109">Наследуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="90ba6-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="90ba6-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="90ba6-110">Properties</span></span>
|<span data-ttu-id="90ba6-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="90ba6-111">Property</span></span>|<span data-ttu-id="90ba6-112">Тип</span><span class="sxs-lookup"><span data-stu-id="90ba6-112">Type</span></span>|<span data-ttu-id="90ba6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="90ba6-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90ba6-114">алловедурлс</span><span class="sxs-lookup"><span data-stu-id="90ba6-114">allowedUrls</span></span>|<span data-ttu-id="90ba6-115">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="90ba6-115">String collection</span></span>|<span data-ttu-id="90ba6-116">Дополнительные URL-адреса, разрешенные для Access</span><span class="sxs-lookup"><span data-stu-id="90ba6-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="90ba6-117">блоккедурлс</span><span class="sxs-lookup"><span data-stu-id="90ba6-117">blockedUrls</span></span>|<span data-ttu-id="90ba6-118">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="90ba6-118">String collection</span></span>|<span data-ttu-id="90ba6-119">Дополнительные URL-адреса, заблокированные для Access</span><span class="sxs-lookup"><span data-stu-id="90ba6-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="90ba6-120">Связи</span><span class="sxs-lookup"><span data-stu-id="90ba6-120">Relationships</span></span>
<span data-ttu-id="90ba6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="90ba6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="90ba6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="90ba6-122">JSON Representation</span></span>
<span data-ttu-id="90ba6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="90ba6-123">Here is a JSON representation of the resource.</span></span>
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



