---
title: Тип ресурса bulkManagedDeviceActionResult
description: Н/Д
author: tfitzmac
ms.openlocfilehash: 0a80a05b1caba7cd5ac1e672c9e39366ca29048c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339517"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="3e929-103">Тип ресурса bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="3e929-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="3e929-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="3e929-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3e929-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3e929-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3e929-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="3e929-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3e929-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="3e929-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="3e929-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3e929-108">Properties</span></span>
|<span data-ttu-id="3e929-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3e929-109">Property</span></span>|<span data-ttu-id="3e929-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3e929-110">Type</span></span>|<span data-ttu-id="3e929-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3e929-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e929-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="3e929-112">successfulDeviceIds</span></span>|<span data-ttu-id="3e929-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e929-113">String collection</span></span>|<span data-ttu-id="3e929-114">Успешные устройств</span><span class="sxs-lookup"><span data-stu-id="3e929-114">Successful devices</span></span>|
|<span data-ttu-id="3e929-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="3e929-115">failedDeviceIds</span></span>|<span data-ttu-id="3e929-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e929-116">String collection</span></span>|<span data-ttu-id="3e929-117">Сбой устройств</span><span class="sxs-lookup"><span data-stu-id="3e929-117">Failed devices</span></span>|
|<span data-ttu-id="3e929-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="3e929-118">notFoundDeviceIds</span></span>|<span data-ttu-id="3e929-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e929-119">String collection</span></span>|<span data-ttu-id="3e929-120">Не найден устройств</span><span class="sxs-lookup"><span data-stu-id="3e929-120">Not found devices</span></span>|
|<span data-ttu-id="3e929-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="3e929-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="3e929-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="3e929-122">String collection</span></span>|<span data-ttu-id="3e929-123">Не поддерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="3e929-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="3e929-124">Связи</span><span class="sxs-lookup"><span data-stu-id="3e929-124">Relationships</span></span>
<span data-ttu-id="3e929-125">Нет</span><span class="sxs-lookup"><span data-stu-id="3e929-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3e929-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3e929-126">JSON Representation</span></span>
<span data-ttu-id="3e929-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3e929-127">Here is a JSON representation of the resource.</span></span>
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





