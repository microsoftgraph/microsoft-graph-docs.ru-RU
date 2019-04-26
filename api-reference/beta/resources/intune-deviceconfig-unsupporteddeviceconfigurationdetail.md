---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 660f73774025a065565fb72ca74c9674a4159fc0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548693"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="b30a4-103">Тип ресурса Унсуппортеддевицеконфигуратиондетаил</span><span class="sxs-lookup"><span data-stu-id="b30a4-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="b30a4-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b30a4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b30a4-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b30a4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b30a4-106">Описание причин неподдерживаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="b30a4-106">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="b30a4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b30a4-107">Properties</span></span>
|<span data-ttu-id="b30a4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b30a4-108">Property</span></span>|<span data-ttu-id="b30a4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b30a4-109">Type</span></span>|<span data-ttu-id="b30a4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b30a4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b30a4-111">message</span><span class="sxs-lookup"><span data-stu-id="b30a4-111">message</span></span>|<span data-ttu-id="b30a4-112">String</span><span class="sxs-lookup"><span data-stu-id="b30a4-112">String</span></span>|<span data-ttu-id="b30a4-113">Сообщение С объяснением, почему объект не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b30a4-113">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="b30a4-114">propertyName</span><span class="sxs-lookup"><span data-stu-id="b30a4-114">propertyName</span></span>|<span data-ttu-id="b30a4-115">String</span><span class="sxs-lookup"><span data-stu-id="b30a4-115">String</span></span>|<span data-ttu-id="b30a4-116">Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="b30a4-116">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b30a4-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="b30a4-117">Relationships</span></span>
<span data-ttu-id="b30a4-118">Нет</span><span class="sxs-lookup"><span data-stu-id="b30a4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b30a4-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b30a4-119">JSON Representation</span></span>
<span data-ttu-id="b30a4-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b30a4-120">Here is a JSON representation of the resource.</span></span>
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





