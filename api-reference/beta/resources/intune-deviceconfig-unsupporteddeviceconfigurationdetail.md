---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f033e30400e3c198f325507030b2267425ce8f80
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48703799"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="ce715-103">Тип ресурса Унсуппортеддевицеконфигуратиондетаил</span><span class="sxs-lookup"><span data-stu-id="ce715-103">unsupportedDeviceConfigurationDetail resource type</span></span>

<span data-ttu-id="ce715-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce715-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce715-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce715-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce715-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ce715-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce715-107">Описание причин неподдерживаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="ce715-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="ce715-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="ce715-108">Properties</span></span>
|<span data-ttu-id="ce715-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="ce715-109">Property</span></span>|<span data-ttu-id="ce715-110">Тип</span><span class="sxs-lookup"><span data-stu-id="ce715-110">Type</span></span>|<span data-ttu-id="ce715-111">Описание</span><span class="sxs-lookup"><span data-stu-id="ce715-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce715-112">message</span><span class="sxs-lookup"><span data-stu-id="ce715-112">message</span></span>|<span data-ttu-id="ce715-113">String</span><span class="sxs-lookup"><span data-stu-id="ce715-113">String</span></span>|<span data-ttu-id="ce715-114">Сообщение с объяснением, почему объект не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ce715-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="ce715-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="ce715-115">propertyName</span></span>|<span data-ttu-id="ce715-116">Строка</span><span class="sxs-lookup"><span data-stu-id="ce715-116">String</span></span>|<span data-ttu-id="ce715-117">Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="ce715-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce715-118">Связи</span><span class="sxs-lookup"><span data-stu-id="ce715-118">Relationships</span></span>
<span data-ttu-id="ce715-119">Нет</span><span class="sxs-lookup"><span data-stu-id="ce715-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce715-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ce715-120">JSON Representation</span></span>
<span data-ttu-id="ce715-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ce715-121">Here is a JSON representation of the resource.</span></span>
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





