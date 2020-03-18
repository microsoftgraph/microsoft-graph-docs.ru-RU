---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 710f71b65a30e8211895c0b0073a572a385a89b7
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787455"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="d63ff-103">Тип ресурса Унсуппортеддевицеконфигуратиондетаил</span><span class="sxs-lookup"><span data-stu-id="d63ff-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="d63ff-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d63ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d63ff-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="d63ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d63ff-106">Описание причин неподдерживаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="d63ff-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="d63ff-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="d63ff-107">Properties</span></span>
|<span data-ttu-id="d63ff-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="d63ff-108">Property</span></span>|<span data-ttu-id="d63ff-109">Тип</span><span class="sxs-lookup"><span data-stu-id="d63ff-109">Type</span></span>|<span data-ttu-id="d63ff-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d63ff-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d63ff-111">message</span><span class="sxs-lookup"><span data-stu-id="d63ff-111">message</span></span>|<span data-ttu-id="d63ff-112">String</span><span class="sxs-lookup"><span data-stu-id="d63ff-112">String</span></span>|<span data-ttu-id="d63ff-113">Сообщение с объяснением, почему объект не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d63ff-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="d63ff-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="d63ff-114">propertyName</span></span>|<span data-ttu-id="d63ff-115">String</span><span class="sxs-lookup"><span data-stu-id="d63ff-115">String</span></span>|<span data-ttu-id="d63ff-116">Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="d63ff-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d63ff-117">Связи</span><span class="sxs-lookup"><span data-stu-id="d63ff-117">Relationships</span></span>
<span data-ttu-id="d63ff-118">Нет</span><span class="sxs-lookup"><span data-stu-id="d63ff-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d63ff-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d63ff-119">JSON Representation</span></span>
<span data-ttu-id="d63ff-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d63ff-120">Here is a JSON representation of the resource.</span></span>
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



