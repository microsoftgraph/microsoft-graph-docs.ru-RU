---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3f22ace5fa4c381584325ffc8434f0e09faaaaeb
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156016"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="4af63-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="4af63-103">auditResource resource type</span></span>

> <span data-ttu-id="4af63-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="4af63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4af63-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="4af63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4af63-106">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="4af63-106">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="4af63-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="4af63-107">Properties</span></span>
|<span data-ttu-id="4af63-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="4af63-108">Property</span></span>|<span data-ttu-id="4af63-109">Тип</span><span class="sxs-lookup"><span data-stu-id="4af63-109">Type</span></span>|<span data-ttu-id="4af63-110">Описание</span><span class="sxs-lookup"><span data-stu-id="4af63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4af63-111">displayName</span><span class="sxs-lookup"><span data-stu-id="4af63-111">displayName</span></span>|<span data-ttu-id="4af63-112">String</span><span class="sxs-lookup"><span data-stu-id="4af63-112">String</span></span>|<span data-ttu-id="4af63-113">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="4af63-113">Display name.</span></span>|
|<span data-ttu-id="4af63-114">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="4af63-114">modifiedProperties</span></span>|<span data-ttu-id="4af63-115">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="4af63-115">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="4af63-116">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="4af63-116">List of modified properties.</span></span>|
|<span data-ttu-id="4af63-117">type</span><span class="sxs-lookup"><span data-stu-id="4af63-117">type</span></span>|<span data-ttu-id="4af63-118">String</span><span class="sxs-lookup"><span data-stu-id="4af63-118">String</span></span>|<span data-ttu-id="4af63-119">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="4af63-119">Audit resource's type.</span></span>|
|<span data-ttu-id="4af63-120">resourceId</span><span class="sxs-lookup"><span data-stu-id="4af63-120">resourceId</span></span>|<span data-ttu-id="4af63-121">String</span><span class="sxs-lookup"><span data-stu-id="4af63-121">String</span></span>|<span data-ttu-id="4af63-122">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="4af63-122">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4af63-123">Связи</span><span class="sxs-lookup"><span data-stu-id="4af63-123">Relationships</span></span>
<span data-ttu-id="4af63-124">Нет</span><span class="sxs-lookup"><span data-stu-id="4af63-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4af63-125">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4af63-125">JSON Representation</span></span>
<span data-ttu-id="4af63-126">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4af63-126">Here is a JSON representation of the resource.</span></span>
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




