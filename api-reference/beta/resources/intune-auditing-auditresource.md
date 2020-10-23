---
title: Тип ресурса auditResource
description: Класс, содержащий свойства ресурса аудита.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: df8d9a0d255f01992d1559ae348882644c88dbcb
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706060"
---
# <a name="auditresource-resource-type"></a><span data-ttu-id="b339f-103">Тип ресурса auditResource</span><span class="sxs-lookup"><span data-stu-id="b339f-103">auditResource resource type</span></span>

<span data-ttu-id="b339f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b339f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b339f-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b339f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b339f-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b339f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b339f-107">Класс, содержащий свойства ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="b339f-107">A class containing the properties for Audit Resource.</span></span>

## <a name="properties"></a><span data-ttu-id="b339f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b339f-108">Properties</span></span>
|<span data-ttu-id="b339f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b339f-109">Property</span></span>|<span data-ttu-id="b339f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b339f-110">Type</span></span>|<span data-ttu-id="b339f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b339f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b339f-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b339f-112">displayName</span></span>|<span data-ttu-id="b339f-113">Строка</span><span class="sxs-lookup"><span data-stu-id="b339f-113">String</span></span>|<span data-ttu-id="b339f-114">Отображаемое имя.</span><span class="sxs-lookup"><span data-stu-id="b339f-114">Display name.</span></span>|
|<span data-ttu-id="b339f-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="b339f-115">modifiedProperties</span></span>|<span data-ttu-id="b339f-116">Коллекция [auditProperty](../resources/intune-auditing-auditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="b339f-116">[auditProperty](../resources/intune-auditing-auditproperty.md) collection</span></span>|<span data-ttu-id="b339f-117">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="b339f-117">List of modified properties.</span></span>|
|<span data-ttu-id="b339f-118">type</span><span class="sxs-lookup"><span data-stu-id="b339f-118">type</span></span>|<span data-ttu-id="b339f-119">Строка</span><span class="sxs-lookup"><span data-stu-id="b339f-119">String</span></span>|<span data-ttu-id="b339f-120">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="b339f-120">Audit resource's type.</span></span>|
|<span data-ttu-id="b339f-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="b339f-121">resourceId</span></span>|<span data-ttu-id="b339f-122">String</span><span class="sxs-lookup"><span data-stu-id="b339f-122">String</span></span>|<span data-ttu-id="b339f-123">ИД ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="b339f-123">Audit resource's Id.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b339f-124">Связи</span><span class="sxs-lookup"><span data-stu-id="b339f-124">Relationships</span></span>
<span data-ttu-id="b339f-125">Нет</span><span class="sxs-lookup"><span data-stu-id="b339f-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b339f-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b339f-126">JSON Representation</span></span>
<span data-ttu-id="b339f-127">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b339f-127">Here is a JSON representation of the resource.</span></span>
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





