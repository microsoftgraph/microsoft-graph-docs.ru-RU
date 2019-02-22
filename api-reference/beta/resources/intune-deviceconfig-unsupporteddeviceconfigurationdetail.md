---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6ebdb6eb91dd64c1605288cc0cb1260f8fe7440a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148470"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="ae320-103">Тип ресурса Унсуппортеддевицеконфигуратиондетаил</span><span class="sxs-lookup"><span data-stu-id="ae320-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="ae320-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae320-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae320-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae320-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae320-106">Описание причин неподдерживаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="ae320-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="ae320-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae320-107">Properties</span></span>
|<span data-ttu-id="ae320-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae320-108">Property</span></span>|<span data-ttu-id="ae320-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ae320-109">Type</span></span>|<span data-ttu-id="ae320-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ae320-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae320-111">message</span><span class="sxs-lookup"><span data-stu-id="ae320-111">message</span></span>|<span data-ttu-id="ae320-112">String</span><span class="sxs-lookup"><span data-stu-id="ae320-112">String</span></span>|<span data-ttu-id="ae320-113">Сообщение С объяснением, почему объект не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae320-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="ae320-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="ae320-114">propertyName</span></span>|<span data-ttu-id="ae320-115">String</span><span class="sxs-lookup"><span data-stu-id="ae320-115">String</span></span>|<span data-ttu-id="ae320-116">Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="ae320-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae320-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="ae320-117">Relationships</span></span>
<span data-ttu-id="ae320-118">Нет</span><span class="sxs-lookup"><span data-stu-id="ae320-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae320-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae320-119">JSON Representation</span></span>
<span data-ttu-id="ae320-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae320-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```




