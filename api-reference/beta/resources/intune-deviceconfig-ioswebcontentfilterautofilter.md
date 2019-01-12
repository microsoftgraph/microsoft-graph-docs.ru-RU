---
title: Тип ресурса iosWebContentFilterAutoFilter
description: Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который позволяет функция автоматического фильтра операций ввода-вывода и для управления доступом к дополнительные URL-адреса. При создании без значения свойства устройства iOS позволит автоматического фильтра вне зависимости от.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 03e3c4f51e673be1e2bada89e06a26048fe4e385
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27916782"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="22041-104">Тип ресурса iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="22041-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="22041-105">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="22041-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22041-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="22041-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22041-107">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="22041-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22041-108">Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который позволяет функция автоматического фильтра операций ввода-вывода и для управления доступом к дополнительные URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="22041-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="22041-109">При создании без значения свойства устройства iOS позволит автоматического фильтра вне зависимости от.</span><span class="sxs-lookup"><span data-stu-id="22041-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>

<span data-ttu-id="22041-110">Наследуется от [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="22041-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="22041-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="22041-111">Properties</span></span>
|<span data-ttu-id="22041-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="22041-112">Property</span></span>|<span data-ttu-id="22041-113">Тип</span><span class="sxs-lookup"><span data-stu-id="22041-113">Type</span></span>|<span data-ttu-id="22041-114">Описание</span><span class="sxs-lookup"><span data-stu-id="22041-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22041-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="22041-115">allowedUrls</span></span>|<span data-ttu-id="22041-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="22041-116">String collection</span></span>|<span data-ttu-id="22041-117">Дополнительные URL-адреса, разрешенных для access</span><span class="sxs-lookup"><span data-stu-id="22041-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="22041-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="22041-118">blockedUrls</span></span>|<span data-ttu-id="22041-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="22041-119">String collection</span></span>|<span data-ttu-id="22041-120">Дополнительные URL-адреса, заблокированные для access</span><span class="sxs-lookup"><span data-stu-id="22041-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="22041-121">Связи</span><span class="sxs-lookup"><span data-stu-id="22041-121">Relationships</span></span>
<span data-ttu-id="22041-122">Нет</span><span class="sxs-lookup"><span data-stu-id="22041-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="22041-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="22041-123">JSON Representation</span></span>
<span data-ttu-id="22041-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="22041-124">Here is a JSON representation of the resource.</span></span>
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





