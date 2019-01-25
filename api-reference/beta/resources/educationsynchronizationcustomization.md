---
title: Тип ресурса educationSynchronizationCustomization
description: 'Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов. Настройка может применяться для всех сущностей, которые синхронизируются. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513608"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="302e3-104">Тип ресурса educationSynchronizationCustomization</span><span class="sxs-lookup"><span data-stu-id="302e3-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="302e3-105">Содержит параметры для настройки синхронизации профилей данных school сущностей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="302e3-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="302e3-106">Настройка может применяться для всех сущностей, которые синхронизируются.</span><span class="sxs-lookup"><span data-stu-id="302e3-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="302e3-107">**Примечание:** Свойство **synchronizationStartDate** применяется только к **StudentEnrollment** сущности.</span><span class="sxs-lookup"><span data-stu-id="302e3-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="302e3-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="302e3-108">Properties</span></span>

| <span data-ttu-id="302e3-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="302e3-109">Property</span></span> | <span data-ttu-id="302e3-110">Тип</span><span class="sxs-lookup"><span data-stu-id="302e3-110">Type</span></span> | <span data-ttu-id="302e3-111">Описание</span><span class="sxs-lookup"><span data-stu-id="302e3-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="302e3-112">**optionalPropertiesToSync**</span><span class="sxs-lookup"><span data-stu-id="302e3-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="302e3-113">Коллекция строк.</span><span class="sxs-lookup"><span data-stu-id="302e3-113">collection of string</span></span> |  <span data-ttu-id="302e3-114">Коллекция имен свойств для синхронизации. Если задано значение null, все свойства будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="302e3-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="302e3-115">**synchronizationStartDate**</span><span class="sxs-lookup"><span data-stu-id="302e3-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="302e3-116">DateTime</span><span class="sxs-lookup"><span data-stu-id="302e3-116">DateTime</span></span> |  <span data-ttu-id="302e3-117">Дата начала для синхронизации.</span><span class="sxs-lookup"><span data-stu-id="302e3-117">The date that the synchronization should start.</span></span> <span data-ttu-id="302e3-118">Это значение необходимо задать в будущем.</span><span class="sxs-lookup"><span data-stu-id="302e3-118">This value should be set to a future date.</span></span> <span data-ttu-id="302e3-119">Если параметр имеет значение null, ресурс будет синхронизирован после завершения настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="302e3-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="302e3-120">**Примечание:** Применяется только к свойству **StudentEnrollment** .</span><span class="sxs-lookup"><span data-stu-id="302e3-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="302e3-121">**isSyncDeferred**</span><span class="sxs-lookup"><span data-stu-id="302e3-121">**isSyncDeferred**</span></span> |<span data-ttu-id="302e3-122">Логическое</span><span class="sxs-lookup"><span data-stu-id="302e3-122">Boolean</span></span> | <span data-ttu-id="302e3-123">Указывает, будет ли синхронизация родительской сущности откладывается на более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="302e3-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="302e3-124">**allowDisplayNameUpdate**</span><span class="sxs-lookup"><span data-stu-id="302e3-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="302e3-125">Логическое</span><span class="sxs-lookup"><span data-stu-id="302e3-125">Boolean</span></span> |  <span data-ttu-id="302e3-126">Указывает, является ли отображаемое имя ресурса может быть перезаписана при синхронизации.</span><span class="sxs-lookup"><span data-stu-id="302e3-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="302e3-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="302e3-127">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{  
    "optionalPropertiesToSync":["String"],
    "synchronizationStartDate": "DateTimeOffset",
    "isSyncDeferred": "Boolean",
    "allowDisplayNameUpdate": "Boolean"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationcustomization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
