---
title: Тип ресурса androidDeviceOwnerKioskModeAppPositionItem
description: Элемент в списке позиций приложения, который задает порядок элементов на управляемом домашнем экране
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 788b7ac612fd025bb778c387be2051769de66ccb
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160625"
---
# <a name="androiddeviceownerkioskmodeapppositionitem-resource-type"></a><span data-ttu-id="baf33-103">Тип ресурса androidDeviceOwnerKioskModeAppPositionItem</span><span class="sxs-lookup"><span data-stu-id="baf33-103">androidDeviceOwnerKioskModeAppPositionItem resource type</span></span>

<span data-ttu-id="baf33-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baf33-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="baf33-105">**Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="baf33-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="baf33-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="baf33-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="baf33-107">Элемент в списке позиций приложения, который задает порядок элементов на управляемом домашнем экране</span><span class="sxs-lookup"><span data-stu-id="baf33-107">An item in the list of app positions that sets the order of items on the Managed Home Screen</span></span>

## <a name="properties"></a><span data-ttu-id="baf33-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="baf33-108">Properties</span></span>
|<span data-ttu-id="baf33-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="baf33-109">Property</span></span>|<span data-ttu-id="baf33-110">Тип</span><span class="sxs-lookup"><span data-stu-id="baf33-110">Type</span></span>|<span data-ttu-id="baf33-111">Описание</span><span class="sxs-lookup"><span data-stu-id="baf33-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baf33-112">position</span><span class="sxs-lookup"><span data-stu-id="baf33-112">position</span></span>|<span data-ttu-id="baf33-113">Int32</span><span class="sxs-lookup"><span data-stu-id="baf33-113">Int32</span></span>|<span data-ttu-id="baf33-114">Положение элемента в сетке.</span><span class="sxs-lookup"><span data-stu-id="baf33-114">Position of the item on the grid.</span></span> <span data-ttu-id="baf33-115">Допустимые значения: от 0 до 999 999 999</span><span class="sxs-lookup"><span data-stu-id="baf33-115">Valid values 0 to 9999999</span></span>|
|<span data-ttu-id="baf33-116">item</span><span class="sxs-lookup"><span data-stu-id="baf33-116">item</span></span>|[<span data-ttu-id="baf33-117">androidDeviceOwnerKioskModeHomeScreenItem</span><span class="sxs-lookup"><span data-stu-id="baf33-117">androidDeviceOwnerKioskModeHomeScreenItem</span></span>](../resources/intune-deviceconfig-androiddeviceownerkioskmodehomescreenitem.md)|<span data-ttu-id="baf33-118">Устроимый элемент</span><span class="sxs-lookup"><span data-stu-id="baf33-118">Item to be arranged</span></span>|

## <a name="relationships"></a><span data-ttu-id="baf33-119">Связи</span><span class="sxs-lookup"><span data-stu-id="baf33-119">Relationships</span></span>
<span data-ttu-id="baf33-120">Нет</span><span class="sxs-lookup"><span data-stu-id="baf33-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="baf33-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="baf33-121">JSON Representation</span></span>
<span data-ttu-id="baf33-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="baf33-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerKioskModeAppPositionItem",
  "position": 1024,
  "item": {
    "@odata.type": "microsoft.graph.androidDeviceOwnerKioskModeWeblink",
    "label": "String",
    "link": "String"
  }
}
```




