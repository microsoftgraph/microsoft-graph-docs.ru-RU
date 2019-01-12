---
title: Тип ресурса bulkManagedDeviceActionResult
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: adc2b2a6b139ad428cb191fe45a3ca7f4192092a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981779"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="ea879-103">Тип ресурса bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="ea879-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="ea879-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="ea879-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ea879-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ea879-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ea879-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="ea879-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea879-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="ea879-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="ea879-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ea879-108">Properties</span></span>
|<span data-ttu-id="ea879-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ea879-109">Property</span></span>|<span data-ttu-id="ea879-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ea879-110">Type</span></span>|<span data-ttu-id="ea879-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ea879-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea879-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ea879-112">successfulDeviceIds</span></span>|<span data-ttu-id="ea879-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea879-113">String collection</span></span>|<span data-ttu-id="ea879-114">Успешные устройств</span><span class="sxs-lookup"><span data-stu-id="ea879-114">Successful devices</span></span>|
|<span data-ttu-id="ea879-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ea879-115">failedDeviceIds</span></span>|<span data-ttu-id="ea879-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea879-116">String collection</span></span>|<span data-ttu-id="ea879-117">Сбой устройств</span><span class="sxs-lookup"><span data-stu-id="ea879-117">Failed devices</span></span>|
|<span data-ttu-id="ea879-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ea879-118">notFoundDeviceIds</span></span>|<span data-ttu-id="ea879-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea879-119">String collection</span></span>|<span data-ttu-id="ea879-120">Не найден устройств</span><span class="sxs-lookup"><span data-stu-id="ea879-120">Not found devices</span></span>|
|<span data-ttu-id="ea879-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="ea879-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="ea879-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="ea879-122">String collection</span></span>|<span data-ttu-id="ea879-123">Не поддерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="ea879-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea879-124">Связи</span><span class="sxs-lookup"><span data-stu-id="ea879-124">Relationships</span></span>
<span data-ttu-id="ea879-125">Нет</span><span class="sxs-lookup"><span data-stu-id="ea879-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="ea879-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ea879-126">JSON Representation</span></span>
<span data-ttu-id="ea879-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ea879-127">Here is a JSON representation of the resource.</span></span>
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





