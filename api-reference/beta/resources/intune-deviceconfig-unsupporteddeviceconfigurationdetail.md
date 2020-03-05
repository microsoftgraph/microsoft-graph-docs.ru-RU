---
title: Тип ресурса Унсуппортеддевицеконфигуратиондетаил
description: Описание причин неподдерживаемого объекта.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6ad1f5b06e9b3890eea2eb754220572436ac94c3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529355"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="c2d39-103">Тип ресурса Унсуппортеддевицеконфигуратиондетаил</span><span class="sxs-lookup"><span data-stu-id="c2d39-103">unsupportedDeviceConfigurationDetail resource type</span></span>

<span data-ttu-id="c2d39-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="c2d39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2d39-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d39-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2d39-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c2d39-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2d39-107">Описание причин неподдерживаемого объекта.</span><span class="sxs-lookup"><span data-stu-id="c2d39-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="c2d39-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2d39-108">Properties</span></span>
|<span data-ttu-id="c2d39-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2d39-109">Property</span></span>|<span data-ttu-id="c2d39-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c2d39-110">Type</span></span>|<span data-ttu-id="c2d39-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c2d39-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2d39-112">message</span><span class="sxs-lookup"><span data-stu-id="c2d39-112">message</span></span>|<span data-ttu-id="c2d39-113">String</span><span class="sxs-lookup"><span data-stu-id="c2d39-113">String</span></span>|<span data-ttu-id="c2d39-114">Сообщение с объяснением, почему объект не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c2d39-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="c2d39-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="c2d39-115">propertyName</span></span>|<span data-ttu-id="c2d39-116">String</span><span class="sxs-lookup"><span data-stu-id="c2d39-116">String</span></span>|<span data-ttu-id="c2d39-117">Если сообщение связано с определенным свойством в исходной сущности, то имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="c2d39-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2d39-118">Связи</span><span class="sxs-lookup"><span data-stu-id="c2d39-118">Relationships</span></span>
<span data-ttu-id="c2d39-119">Нет</span><span class="sxs-lookup"><span data-stu-id="c2d39-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2d39-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2d39-120">JSON Representation</span></span>
<span data-ttu-id="c2d39-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2d39-121">Here is a JSON representation of the resource.</span></span>
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



