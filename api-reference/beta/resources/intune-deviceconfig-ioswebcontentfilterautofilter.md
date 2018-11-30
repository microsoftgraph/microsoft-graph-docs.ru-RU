---
title: Тип ресурса iosWebContentFilterAutoFilter
description: Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который позволяет функция автоматического фильтра операций ввода-вывода и для управления доступом к дополнительные URL-адреса. При создании без значения свойства устройства iOS позволит автоматического фильтра вне зависимости от.
ms.openlocfilehash: 04a221ac512ab3934702a2a9e3178ba23a2ac3ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27080414"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="4eb28-104">Тип ресурса iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="4eb28-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="4eb28-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="4eb28-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4eb28-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4eb28-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4eb28-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="4eb28-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4eb28-108">Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который позволяет функция автоматического фильтра операций ввода-вывода и для управления доступом к дополнительные URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="4eb28-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="4eb28-109">При создании без значения свойства устройства iOS позволит автоматического фильтра вне зависимости от.</span><span class="sxs-lookup"><span data-stu-id="4eb28-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>

<span data-ttu-id="4eb28-110">Наследуется от [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="4eb28-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="4eb28-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="4eb28-111">Properties</span></span>
|<span data-ttu-id="4eb28-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="4eb28-112">Property</span></span>|<span data-ttu-id="4eb28-113">Тип</span><span class="sxs-lookup"><span data-stu-id="4eb28-113">Type</span></span>|<span data-ttu-id="4eb28-114">Description</span><span class="sxs-lookup"><span data-stu-id="4eb28-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eb28-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="4eb28-115">allowedUrls</span></span>|<span data-ttu-id="4eb28-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4eb28-116">String collection</span></span>|<span data-ttu-id="4eb28-117">Дополнительные URL-адреса, разрешенных для access</span><span class="sxs-lookup"><span data-stu-id="4eb28-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="4eb28-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="4eb28-118">blockedUrls</span></span>|<span data-ttu-id="4eb28-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="4eb28-119">String collection</span></span>|<span data-ttu-id="4eb28-120">Дополнительные URL-адреса, заблокированные для access</span><span class="sxs-lookup"><span data-stu-id="4eb28-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="4eb28-121">Связи</span><span class="sxs-lookup"><span data-stu-id="4eb28-121">Relationships</span></span>
<span data-ttu-id="4eb28-122">Нет</span><span class="sxs-lookup"><span data-stu-id="4eb28-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4eb28-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4eb28-123">JSON Representation</span></span>
<span data-ttu-id="4eb28-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4eb28-124">Here is a JSON representation of the resource.</span></span>
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





