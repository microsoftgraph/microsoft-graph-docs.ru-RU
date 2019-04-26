---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e2a6b2309e831a872c4cde04a951819cac292ec
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534348"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="89f21-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="89f21-103">auditResource resource type</span></span>

> <span data-ttu-id="89f21-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="89f21-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89f21-105">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="89f21-105">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="89f21-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="89f21-106">Properties</span></span>
|<span data-ttu-id="89f21-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="89f21-107">Property</span></span>|<span data-ttu-id="89f21-108">Тип</span><span class="sxs-lookup"><span data-stu-id="89f21-108">Type</span></span>|<span data-ttu-id="89f21-109">Описание</span><span class="sxs-lookup"><span data-stu-id="89f21-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89f21-110">displayName</span><span class="sxs-lookup"><span data-stu-id="89f21-110">displayName</span></span>|<span data-ttu-id="89f21-111">String</span><span class="sxs-lookup"><span data-stu-id="89f21-111">String</span></span>|<span data-ttu-id="89f21-112">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="89f21-112">Display name.</span></span>|
|<span data-ttu-id="89f21-113">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="89f21-113">modifiedProperties</span></span>|<span data-ttu-id="89f21-114">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="89f21-114">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="89f21-115">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="89f21-115">List of modified properties.</span></span>|
|<span data-ttu-id="89f21-116">type</span><span class="sxs-lookup"><span data-stu-id="89f21-116">type</span></span>|<span data-ttu-id="89f21-117">Строка</span><span class="sxs-lookup"><span data-stu-id="89f21-117">String</span></span>|<span data-ttu-id="89f21-118">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="89f21-118">Audit resource's type.</span></span>|
|<span data-ttu-id="89f21-119">resourceId</span><span class="sxs-lookup"><span data-stu-id="89f21-119">resourceId</span></span>|<span data-ttu-id="89f21-120">String</span><span class="sxs-lookup"><span data-stu-id="89f21-120">String</span></span>|<span data-ttu-id="89f21-121">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="89f21-121">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89f21-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="89f21-122">Relationships</span></span>
<span data-ttu-id="89f21-123">Нет</span><span class="sxs-lookup"><span data-stu-id="89f21-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="89f21-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="89f21-124">JSON Representation</span></span>
<span data-ttu-id="89f21-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="89f21-125">Here is a JSON representation of the resource.</span></span>
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



