---
title: Тип ресурса bulkManagedDeviceActionResult
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5d1b23efdb5b8eed16c6c66d72a13efaef9e38d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425843"
---
# <a name="bulkmanageddeviceactionresult-resource-type"></a><span data-ttu-id="e436c-103">Тип ресурса bulkManagedDeviceActionResult</span><span class="sxs-lookup"><span data-stu-id="e436c-103">bulkManagedDeviceActionResult resource type</span></span>

> <span data-ttu-id="e436c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e436c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e436c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e436c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e436c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e436c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e436c-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e436c-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e436c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e436c-108">Properties</span></span>
|<span data-ttu-id="e436c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e436c-109">Property</span></span>|<span data-ttu-id="e436c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e436c-110">Type</span></span>|<span data-ttu-id="e436c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e436c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e436c-112">successfulDeviceIds</span><span class="sxs-lookup"><span data-stu-id="e436c-112">successfulDeviceIds</span></span>|<span data-ttu-id="e436c-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e436c-113">String collection</span></span>|<span data-ttu-id="e436c-114">Успешные устройств</span><span class="sxs-lookup"><span data-stu-id="e436c-114">Successful devices</span></span>|
|<span data-ttu-id="e436c-115">failedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="e436c-115">failedDeviceIds</span></span>|<span data-ttu-id="e436c-116">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e436c-116">String collection</span></span>|<span data-ttu-id="e436c-117">Сбой устройств</span><span class="sxs-lookup"><span data-stu-id="e436c-117">Failed devices</span></span>|
|<span data-ttu-id="e436c-118">notFoundDeviceIds</span><span class="sxs-lookup"><span data-stu-id="e436c-118">notFoundDeviceIds</span></span>|<span data-ttu-id="e436c-119">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e436c-119">String collection</span></span>|<span data-ttu-id="e436c-120">Не найден устройств</span><span class="sxs-lookup"><span data-stu-id="e436c-120">Not found devices</span></span>|
|<span data-ttu-id="e436c-121">notSupportedDeviceIds</span><span class="sxs-lookup"><span data-stu-id="e436c-121">notSupportedDeviceIds</span></span>|<span data-ttu-id="e436c-122">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e436c-122">String collection</span></span>|<span data-ttu-id="e436c-123">Не поддерживаемые устройства</span><span class="sxs-lookup"><span data-stu-id="e436c-123">Not supported devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="e436c-124">Отношения</span><span class="sxs-lookup"><span data-stu-id="e436c-124">Relationships</span></span>
<span data-ttu-id="e436c-125">Нет</span><span class="sxs-lookup"><span data-stu-id="e436c-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e436c-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e436c-126">JSON Representation</span></span>
<span data-ttu-id="e436c-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e436c-127">Here is a JSON representation of the resource.</span></span>
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




