---
title: Тип ресурса Иосвебконтентфилтераутофилтер
description: Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-АДРЕСу. При создании без значений свойств устройство iOS включит автоматический фильтр независимо.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 91efedb47fff71a66d12e0d2c976d61fab2fa76c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460417"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="b3fc6-104">Тип ресурса Иосвебконтентфилтераутофилтер</span><span class="sxs-lookup"><span data-stu-id="b3fc6-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="b3fc6-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3fc6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3fc6-106">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3fc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3fc6-107">Представляет тип параметра фильтра веб-содержимого iOS, который включает функцию автоматического фильтра iOS и предоставляет дополнительные возможности управления доступом по URL-АДРЕСу.</span><span class="sxs-lookup"><span data-stu-id="b3fc6-107">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="b3fc6-108">При создании без значений свойств устройство iOS включит автоматический фильтр независимо.</span><span class="sxs-lookup"><span data-stu-id="b3fc6-108">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="b3fc6-109">НаСледуется от [иосвебконтентфилтербасе](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="b3fc6-109">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b3fc6-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3fc6-110">Properties</span></span>
|<span data-ttu-id="b3fc6-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3fc6-111">Property</span></span>|<span data-ttu-id="b3fc6-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b3fc6-112">Type</span></span>|<span data-ttu-id="b3fc6-113">Описание</span><span class="sxs-lookup"><span data-stu-id="b3fc6-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3fc6-114">Алловедурлс</span><span class="sxs-lookup"><span data-stu-id="b3fc6-114">allowedUrls</span></span>|<span data-ttu-id="b3fc6-115">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b3fc6-115">String collection</span></span>|<span data-ttu-id="b3fc6-116">Дополнительные URL-адреса, разрешенные для Access</span><span class="sxs-lookup"><span data-stu-id="b3fc6-116">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="b3fc6-117">Блоккедурлс</span><span class="sxs-lookup"><span data-stu-id="b3fc6-117">blockedUrls</span></span>|<span data-ttu-id="b3fc6-118">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="b3fc6-118">String collection</span></span>|<span data-ttu-id="b3fc6-119">Дополнительные URL-адреса, заблокированные для Access</span><span class="sxs-lookup"><span data-stu-id="b3fc6-119">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3fc6-120">Отношения</span><span class="sxs-lookup"><span data-stu-id="b3fc6-120">Relationships</span></span>
<span data-ttu-id="b3fc6-121">Нет</span><span class="sxs-lookup"><span data-stu-id="b3fc6-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3fc6-122">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3fc6-122">JSON Representation</span></span>
<span data-ttu-id="b3fc6-123">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3fc6-123">Here is a JSON representation of the resource.</span></span>
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





