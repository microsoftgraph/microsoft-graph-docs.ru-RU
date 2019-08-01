---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 14ecd6e4772e6d694707bd047899bd6b75720252
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028863"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="6eb68-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="6eb68-103">auditResource resource type</span></span>

> <span data-ttu-id="6eb68-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6eb68-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6eb68-105">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="6eb68-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="6eb68-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="6eb68-106">Properties</span></span>
|<span data-ttu-id="6eb68-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="6eb68-107">Property</span></span>|<span data-ttu-id="6eb68-108">Тип</span><span class="sxs-lookup"><span data-stu-id="6eb68-108">Type</span></span>|<span data-ttu-id="6eb68-109">Описание</span><span class="sxs-lookup"><span data-stu-id="6eb68-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eb68-110">displayName</span><span class="sxs-lookup"><span data-stu-id="6eb68-110">displayName</span></span>|<span data-ttu-id="6eb68-111">Строка</span><span class="sxs-lookup"><span data-stu-id="6eb68-111">String</span></span>|<span data-ttu-id="6eb68-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="6eb68-112">Display name.</span></span>|
|<span data-ttu-id="6eb68-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="6eb68-113">modifiedProperties</span></span>|<span data-ttu-id="6eb68-114">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="6eb68-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="6eb68-115">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="6eb68-115">List of modified properties.</span></span>|
|<span data-ttu-id="6eb68-116">type</span><span class="sxs-lookup"><span data-stu-id="6eb68-116">type</span></span>|<span data-ttu-id="6eb68-117">String</span><span class="sxs-lookup"><span data-stu-id="6eb68-117">String</span></span>|<span data-ttu-id="6eb68-118">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="6eb68-118">Audit resource's type.</span></span>|
|<span data-ttu-id="6eb68-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="6eb68-119">resourceId</span></span>|<span data-ttu-id="6eb68-120">String</span><span class="sxs-lookup"><span data-stu-id="6eb68-120">String</span></span>|<span data-ttu-id="6eb68-121">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="6eb68-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6eb68-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="6eb68-122">Relationships</span></span>
<span data-ttu-id="6eb68-123">Нет</span><span class="sxs-lookup"><span data-stu-id="6eb68-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6eb68-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6eb68-124">JSON Representation</span></span>
<span data-ttu-id="6eb68-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6eb68-125">Here is a JSON representation of the resource.</span></span>
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



