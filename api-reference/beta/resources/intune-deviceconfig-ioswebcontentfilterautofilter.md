---
title: Тип ресурса iosWebContentFilterAutoFilter
description: Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который позволяет функция автоматического фильтра операций ввода-вывода и для управления доступом к дополнительные URL-адреса. При создании без значения свойства устройства iOS позволит автоматического фильтра вне зависимости от.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5be275b74e2675881b9d36b047e2017ef95adb2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401231"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a><span data-ttu-id="363a6-104">Тип ресурса iosWebContentFilterAutoFilter</span><span class="sxs-lookup"><span data-stu-id="363a6-104">iosWebContentFilterAutoFilter resource type</span></span>

> <span data-ttu-id="363a6-105">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="363a6-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="363a6-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="363a6-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="363a6-107">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="363a6-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="363a6-108">Представляет операций ввода-вывода тип параметра фильтра веб-содержимого, который позволяет функция автоматического фильтра операций ввода-вывода и для управления доступом к дополнительные URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="363a6-108">Represents an iOS Web Content Filter setting type, which enables iOS automatic filter feature and allows for additional URL access control.</span></span> <span data-ttu-id="363a6-109">При создании без значения свойства устройства iOS позволит автоматического фильтра вне зависимости от.</span><span class="sxs-lookup"><span data-stu-id="363a6-109">When constructed with no property values, the iOS device will enable the automatic filter regardless.</span></span>


<span data-ttu-id="363a6-110">Наследуется от [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span><span class="sxs-lookup"><span data-stu-id="363a6-110">Inherits from [iosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="363a6-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="363a6-111">Properties</span></span>
|<span data-ttu-id="363a6-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="363a6-112">Property</span></span>|<span data-ttu-id="363a6-113">Тип</span><span class="sxs-lookup"><span data-stu-id="363a6-113">Type</span></span>|<span data-ttu-id="363a6-114">Описание</span><span class="sxs-lookup"><span data-stu-id="363a6-114">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="363a6-115">allowedUrls</span><span class="sxs-lookup"><span data-stu-id="363a6-115">allowedUrls</span></span>|<span data-ttu-id="363a6-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="363a6-116">String collection</span></span>|<span data-ttu-id="363a6-117">Дополнительные URL-адреса, разрешенных для access</span><span class="sxs-lookup"><span data-stu-id="363a6-117">Additional URLs allowed for access</span></span>|
|<span data-ttu-id="363a6-118">blockedUrls</span><span class="sxs-lookup"><span data-stu-id="363a6-118">blockedUrls</span></span>|<span data-ttu-id="363a6-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="363a6-119">String collection</span></span>|<span data-ttu-id="363a6-120">Дополнительные URL-адреса, заблокированные для access</span><span class="sxs-lookup"><span data-stu-id="363a6-120">Additional URLs blocked for access</span></span>|

## <a name="relationships"></a><span data-ttu-id="363a6-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="363a6-121">Relationships</span></span>
<span data-ttu-id="363a6-122">Нет</span><span class="sxs-lookup"><span data-stu-id="363a6-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="363a6-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="363a6-123">JSON Representation</span></span>
<span data-ttu-id="363a6-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="363a6-124">Here is a JSON representation of the resource.</span></span>
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




