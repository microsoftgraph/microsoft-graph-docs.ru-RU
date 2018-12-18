---
title: Тип ресурса educationSynchronizationCustomization
description: 'Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. '
author: mmast-msft
ms.openlocfilehash: d4f67c9f56198350731c18fe3da8b512522c4d71
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350638"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="dbad2-104">Тип ресурса educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="dbad2-104">educationSynchronizationCustomization resource type</span></span>

> <span data-ttu-id="dbad2-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="dbad2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbad2-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="dbad2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbad2-107">Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="dbad2-107">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="dbad2-108">Настройка может применяться для всех сущностей, которые синхронизируются.</span><span class="sxs-lookup"><span data-stu-id="dbad2-108">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="dbad2-109">**Примечание:** Свойство **synchronizationStartDate** применяется только к **StudentEnrollment** сущности.</span><span class="sxs-lookup"><span data-stu-id="dbad2-109">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="dbad2-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="dbad2-110">Properties</span></span>

| <span data-ttu-id="dbad2-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="dbad2-111">Property</span></span> | <span data-ttu-id="dbad2-112">Тип</span><span class="sxs-lookup"><span data-stu-id="dbad2-112">Type</span></span> | <span data-ttu-id="dbad2-113">Описание</span><span class="sxs-lookup"><span data-stu-id="dbad2-113">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="dbad2-114">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="dbad2-114">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="dbad2-115">Набор типа string</span><span class="sxs-lookup"><span data-stu-id="dbad2-115">collection of string</span></span> |  <span data-ttu-id="dbad2-116">Коллекция имен свойств для синхронизации. Если задано значение null, все свойства будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="dbad2-116">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="dbad2-117">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="dbad2-117">**synchronizationStartDate**</span></span> | <span data-ttu-id="dbad2-118">DateTime.</span><span class="sxs-lookup"><span data-stu-id="dbad2-118">DateTime</span></span> |  <span data-ttu-id="dbad2-119">Дата начала для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dbad2-119">The date that the synchronization should start.</span></span> <span data-ttu-id="dbad2-120">Это значение необходимо задать в будущем.</span><span class="sxs-lookup"><span data-stu-id="dbad2-120">This value should be set to a future date.</span></span> <span data-ttu-id="dbad2-121">Если параметр имеет значение null, ресурс будет синхронизирован после завершения настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="dbad2-121">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="dbad2-122">**Примечание:** Применяется только к свойству **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="dbad2-122">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="dbad2-123">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="dbad2-123">**isSyncDeferred**</span></span> |<span data-ttu-id="dbad2-124">Boolean.</span><span class="sxs-lookup"><span data-stu-id="dbad2-124">Boolean</span></span> | <span data-ttu-id="dbad2-125">Указывает, будет ли синхронизация родительской сущности откладывается на более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="dbad2-125">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="dbad2-126">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="dbad2-126">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="dbad2-127">Boolean.</span><span class="sxs-lookup"><span data-stu-id="dbad2-127">Boolean</span></span> |  <span data-ttu-id="dbad2-128">Указывает, является ли отображаемое имя ресурса может быть перезаписана при синхронизации.</span><span class="sxs-lookup"><span data-stu-id="dbad2-128">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="dbad2-129">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="dbad2-129">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
