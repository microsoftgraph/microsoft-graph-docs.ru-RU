---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfb4a25325826b20f77d75dc9d545ee64d12f254
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33944651"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="360a7-103">Тип ресурса Унсуппортеддевицеконфигуратиондетаил</span><span class="sxs-lookup"><span data-stu-id="360a7-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="360a7-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="360a7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="360a7-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="360a7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="360a7-106">Описание причин неподдерживаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="360a7-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="360a7-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="360a7-107">Properties</span></span>
|<span data-ttu-id="360a7-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="360a7-108">Property</span></span>|<span data-ttu-id="360a7-109">Тип</span><span class="sxs-lookup"><span data-stu-id="360a7-109">Type</span></span>|<span data-ttu-id="360a7-110">Описание</span><span class="sxs-lookup"><span data-stu-id="360a7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="360a7-111">message</span><span class="sxs-lookup"><span data-stu-id="360a7-111">message</span></span>|<span data-ttu-id="360a7-112">String</span><span class="sxs-lookup"><span data-stu-id="360a7-112">String</span></span>|<span data-ttu-id="360a7-113">Сообщение С объяснением, почему объект не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="360a7-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="360a7-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="360a7-114">propertyName</span></span>|<span data-ttu-id="360a7-115">Строка</span><span class="sxs-lookup"><span data-stu-id="360a7-115">String</span></span>|<span data-ttu-id="360a7-116">Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="360a7-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="360a7-117">Связи</span><span class="sxs-lookup"><span data-stu-id="360a7-117">Relationships</span></span>
<span data-ttu-id="360a7-118">Нет</span><span class="sxs-lookup"><span data-stu-id="360a7-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="360a7-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="360a7-119">JSON Representation</span></span>
<span data-ttu-id="360a7-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="360a7-120">Here is a JSON representation of the resource.</span></span>
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




