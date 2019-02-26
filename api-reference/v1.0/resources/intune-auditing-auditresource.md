---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e2a6b2309e831a872c4cde04a951819cac292ec
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262085"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="93ca4-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="93ca4-103">auditResource resource type</span></span>

> <span data-ttu-id="93ca4-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="93ca4-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93ca4-105">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="93ca4-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="93ca4-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="93ca4-106">Properties</span></span>
|<span data-ttu-id="93ca4-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="93ca4-107">Property</span></span>|<span data-ttu-id="93ca4-108">Тип</span><span class="sxs-lookup"><span data-stu-id="93ca4-108">Type</span></span>|<span data-ttu-id="93ca4-109">Описание</span><span class="sxs-lookup"><span data-stu-id="93ca4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93ca4-110">displayName</span><span class="sxs-lookup"><span data-stu-id="93ca4-110">displayName</span></span>|<span data-ttu-id="93ca4-111">String</span><span class="sxs-lookup"><span data-stu-id="93ca4-111">String</span></span>|<span data-ttu-id="93ca4-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="93ca4-112">Display name.</span></span>|
|<span data-ttu-id="93ca4-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="93ca4-113">modifiedProperties</span></span>|<span data-ttu-id="93ca4-114">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="93ca4-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="93ca4-115">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="93ca4-115">List of modified properties.</span></span>|
|<span data-ttu-id="93ca4-116">type</span><span class="sxs-lookup"><span data-stu-id="93ca4-116">type</span></span>|<span data-ttu-id="93ca4-117">String</span><span class="sxs-lookup"><span data-stu-id="93ca4-117">String</span></span>|<span data-ttu-id="93ca4-118">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="93ca4-118">Audit resource's type.</span></span>|
|<span data-ttu-id="93ca4-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="93ca4-119">resourceId</span></span>|<span data-ttu-id="93ca4-120">String</span><span class="sxs-lookup"><span data-stu-id="93ca4-120">String</span></span>|<span data-ttu-id="93ca4-121">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="93ca4-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="93ca4-122">Связи</span><span class="sxs-lookup"><span data-stu-id="93ca4-122">Relationships</span></span>
<span data-ttu-id="93ca4-123">Нет</span><span class="sxs-lookup"><span data-stu-id="93ca4-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="93ca4-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="93ca4-124">JSON Representation</span></span>
<span data-ttu-id="93ca4-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="93ca4-125">Here is a JSON representation of the resource.</span></span>
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



