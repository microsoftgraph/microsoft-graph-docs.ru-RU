---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d628fb6c7bc8adfab97b401d9ebc8879435502c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367822"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="72c3d-103">Тип ресурса Унсуппортеддевицеконфигуратиондетаил</span><span class="sxs-lookup"><span data-stu-id="72c3d-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="72c3d-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c3d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72c3d-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="72c3d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72c3d-106">Описание причин неподдерживаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="72c3d-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="72c3d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="72c3d-107">Properties</span></span>
|<span data-ttu-id="72c3d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="72c3d-108">Property</span></span>|<span data-ttu-id="72c3d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="72c3d-109">Type</span></span>|<span data-ttu-id="72c3d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="72c3d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72c3d-111">message</span><span class="sxs-lookup"><span data-stu-id="72c3d-111">message</span></span>|<span data-ttu-id="72c3d-112">String</span><span class="sxs-lookup"><span data-stu-id="72c3d-112">String</span></span>|<span data-ttu-id="72c3d-113">Сообщение с объяснением, почему объект не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="72c3d-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="72c3d-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="72c3d-114">propertyName</span></span>|<span data-ttu-id="72c3d-115">String</span><span class="sxs-lookup"><span data-stu-id="72c3d-115">String</span></span>|<span data-ttu-id="72c3d-116">Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="72c3d-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72c3d-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="72c3d-117">Relationships</span></span>
<span data-ttu-id="72c3d-118">Нет</span><span class="sxs-lookup"><span data-stu-id="72c3d-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72c3d-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="72c3d-119">JSON Representation</span></span>
<span data-ttu-id="72c3d-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="72c3d-120">Here is a JSON representation of the resource.</span></span>
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



