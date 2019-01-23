---
title: Тип ресурса unsupportedDeviceConfigurationDetail
description: Описание причины сущности не поддерживается.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c03bdb20fc4c48fa7820e09b9212bf73250599aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400391"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="bb0ad-103">Тип ресурса unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="bb0ad-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="bb0ad-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bb0ad-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bb0ad-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb0ad-107">Описание причины сущности не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-107">A description of why an entity is unsupported.</span></span>

## <a name="properties"></a><span data-ttu-id="bb0ad-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="bb0ad-108">Properties</span></span>
|<span data-ttu-id="bb0ad-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="bb0ad-109">Property</span></span>|<span data-ttu-id="bb0ad-110">Тип</span><span class="sxs-lookup"><span data-stu-id="bb0ad-110">Type</span></span>|<span data-ttu-id="bb0ad-111">Описание</span><span class="sxs-lookup"><span data-stu-id="bb0ad-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb0ad-112">message</span><span class="sxs-lookup"><span data-stu-id="bb0ad-112">message</span></span>|<span data-ttu-id="bb0ad-113">String</span><span class="sxs-lookup"><span data-stu-id="bb0ad-113">String</span></span>|<span data-ttu-id="bb0ad-114">Сообщение о том, почему сущности не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="bb0ad-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="bb0ad-115">propertyName</span></span>|<span data-ttu-id="bb0ad-116">String</span><span class="sxs-lookup"><span data-stu-id="bb0ad-116">String</span></span>|<span data-ttu-id="bb0ad-117">Если сообщение относится к определенное свойство в исходной сущности, а затем имя этого свойства.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb0ad-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="bb0ad-118">Relationships</span></span>
<span data-ttu-id="bb0ad-119">Нет</span><span class="sxs-lookup"><span data-stu-id="bb0ad-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb0ad-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bb0ad-120">JSON Representation</span></span>
<span data-ttu-id="bb0ad-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bb0ad-121">Here is a JSON representation of the resource.</span></span>
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




