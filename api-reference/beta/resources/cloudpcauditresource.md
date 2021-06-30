---
title: тип ресурса cloudPcAuditResource
description: Представляет ресурс аудита.Это показывает объект целевого редактирования ресурсов с несколькими измененными свойствами.
author: ecmadao
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: ebd61a14680c5e5f2917e273456bcce60672149e
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211404"
---
# <a name="cloudpcauditresource-resource-type"></a><span data-ttu-id="c1bc6-104">тип ресурса cloudPcAuditResource</span><span class="sxs-lookup"><span data-stu-id="c1bc6-104">cloudPcAuditResource resource type</span></span>

<span data-ttu-id="c1bc6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1bc6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1bc6-106">Представляет ресурс аудита.</span><span class="sxs-lookup"><span data-stu-id="c1bc6-106">Represents the audit resource.</span></span><span data-ttu-id="c1bc6-107">Это показывает объект целевого редактирования ресурсов с несколькими измененными свойствами.</span><span class="sxs-lookup"><span data-stu-id="c1bc6-107"> This shows the target edited resource entity, with multiple edited properties.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="properties"></a><span data-ttu-id="c1bc6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c1bc6-108">Properties</span></span>
|<span data-ttu-id="c1bc6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c1bc6-109">Property</span></span>|<span data-ttu-id="c1bc6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c1bc6-110">Type</span></span>|<span data-ttu-id="c1bc6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c1bc6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c1bc6-112">displayName</span><span class="sxs-lookup"><span data-stu-id="c1bc6-112">displayName</span></span>|<span data-ttu-id="c1bc6-113">String</span><span class="sxs-lookup"><span data-stu-id="c1bc6-113">String</span></span>|<span data-ttu-id="c1bc6-114">Отображает имя объекта ресурса.</span><span class="sxs-lookup"><span data-stu-id="c1bc6-114">The resource entity display name.</span></span>|
|<span data-ttu-id="c1bc6-115">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="c1bc6-115">modifiedProperties</span></span>|<span data-ttu-id="c1bc6-116">[коллекция cloudPcAuditProperty](../resources/cloudpcauditproperty.md)</span><span class="sxs-lookup"><span data-stu-id="c1bc6-116">[cloudPcAuditProperty](../resources/cloudpcauditproperty.md) collection</span></span>|<span data-ttu-id="c1bc6-117">Список измененных свойств.</span><span class="sxs-lookup"><span data-stu-id="c1bc6-117">A list of modified properties.</span></span>|
|<span data-ttu-id="c1bc6-118">type</span><span class="sxs-lookup"><span data-stu-id="c1bc6-118">type</span></span>|<span data-ttu-id="c1bc6-119">String</span><span class="sxs-lookup"><span data-stu-id="c1bc6-119">String</span></span>|<span data-ttu-id="c1bc6-120">Тип ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="c1bc6-120">The type of the audit resource.</span></span>|
|<span data-ttu-id="c1bc6-121">resourceId</span><span class="sxs-lookup"><span data-stu-id="c1bc6-121">resourceId</span></span>|<span data-ttu-id="c1bc6-122">String</span><span class="sxs-lookup"><span data-stu-id="c1bc6-122">String</span></span>|<span data-ttu-id="c1bc6-123">ID ресурса аудита.</span><span class="sxs-lookup"><span data-stu-id="c1bc6-123">The ID of the audit resource.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c1bc6-124">Связи</span><span class="sxs-lookup"><span data-stu-id="c1bc6-124">Relationships</span></span>

<span data-ttu-id="c1bc6-125">Нет</span><span class="sxs-lookup"><span data-stu-id="c1bc6-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1bc6-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c1bc6-126">JSON Representation</span></span>

<span data-ttu-id="c1bc6-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c1bc6-127">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcAuditResource"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcAuditResource",
  "displayName": "String",
  "modifiedProperties": [
    {
      "@odata.type": "microsoft.graph.cloudPcAuditProperty",
      "displayName": "String",
      "oldValue": "String",
      "newValue": "String"
    }
  ],
  "type": "String",
  "resourceId": "String"
}
```
