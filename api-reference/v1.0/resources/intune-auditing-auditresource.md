---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 35d4385ca16569e1b7e0177995c32ae22e5a0aa0
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43439489"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="f565c-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="f565c-103">auditResource resource type</span></span>

<span data-ttu-id="f565c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f565c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f565c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f565c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f565c-106">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="f565c-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="f565c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="f565c-107">Properties</span></span>
|<span data-ttu-id="f565c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="f565c-108">Property</span></span>|<span data-ttu-id="f565c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="f565c-109">Type</span></span>|<span data-ttu-id="f565c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f565c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f565c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="f565c-111">displayName</span></span>|<span data-ttu-id="f565c-112">Строка</span><span class="sxs-lookup"><span data-stu-id="f565c-112">String</span></span>|<span data-ttu-id="f565c-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="f565c-113">Display name.</span></span>|
|<span data-ttu-id="f565c-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="f565c-114">modifiedProperties</span></span>|<span data-ttu-id="f565c-115">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="f565c-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="f565c-116">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="f565c-116">List of modified properties.</span></span>|
|<span data-ttu-id="f565c-117">type</span><span class="sxs-lookup"><span data-stu-id="f565c-117">type</span></span>|<span data-ttu-id="f565c-118">String</span><span class="sxs-lookup"><span data-stu-id="f565c-118">String</span></span>|<span data-ttu-id="f565c-119">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="f565c-119">Audit resource's type.</span></span>|
|<span data-ttu-id="f565c-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="f565c-120">resourceId</span></span>|<span data-ttu-id="f565c-121">String</span><span class="sxs-lookup"><span data-stu-id="f565c-121">String</span></span>|<span data-ttu-id="f565c-122">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="f565c-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f565c-123">Отношения</span><span class="sxs-lookup"><span data-stu-id="f565c-123">Relationships</span></span>
<span data-ttu-id="f565c-124">Нет</span><span class="sxs-lookup"><span data-stu-id="f565c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f565c-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f565c-125">JSON Representation</span></span>
<span data-ttu-id="f565c-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f565c-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditResource"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.auditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```







