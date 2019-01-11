---
title: Тип ресурса bulkManagedDeviceActionResult
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c7aa0d49182908a960130e202fd4cf096c2c16c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872249"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="04430-103">Тип ресурса bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="04430-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="04430-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="04430-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="04430-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="04430-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04430-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="04430-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04430-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="04430-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="04430-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="04430-108">Properties</span></span>
|<span data-ttu-id="04430-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="04430-109">Property</span></span>|<span data-ttu-id="04430-110">Тип</span><span class="sxs-lookup"><span data-stu-id="04430-110">Type</span></span>|<span data-ttu-id="04430-111">Описание</span><span class="sxs-lookup"><span data-stu-id="04430-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04430-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="04430-112">successfulDeviceIds</span></span>|<span data-ttu-id="04430-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04430-113">String collection</span></span>|<span data-ttu-id="04430-114">Успешные устройств</span><span class="sxs-lookup"><span data-stu-id="04430-114">Successful devices</span></span>|
|<span data-ttu-id="04430-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="04430-115">failedDeviceIds</span></span>|<span data-ttu-id="04430-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04430-116">String collection</span></span>|<span data-ttu-id="04430-117">Сбой устройств</span><span class="sxs-lookup"><span data-stu-id="04430-117">Failed devices</span></span>|
|<span data-ttu-id="04430-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="04430-118">notFoundDeviceIds</span></span>|<span data-ttu-id="04430-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04430-119">String collection</span></span>|<span data-ttu-id="04430-120">Не найден устройств</span><span class="sxs-lookup"><span data-stu-id="04430-120">Not found devices</span></span>|
|<span data-ttu-id="04430-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="04430-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="04430-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="04430-122">String collection</span></span>|<span data-ttu-id="04430-123">Не поддерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="04430-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="04430-124">Связи</span><span class="sxs-lookup"><span data-stu-id="04430-124">Relationships</span></span>
<span data-ttu-id="04430-125">Нет</span><span class="sxs-lookup"><span data-stu-id="04430-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="04430-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="04430-126">JSON Representation</span></span>
<span data-ttu-id="04430-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="04430-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bulkManagedDeviceActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bulkManagedDeviceActionResult",
  "successfulDeviceIds": [
    "String"
  ],
  "failedDeviceIds": [
    "String"
  ],
  "notFoundDeviceIds": [
    "String"
  ],
  "notSupportedDeviceIds": [
    "String"
  ]
}
```





