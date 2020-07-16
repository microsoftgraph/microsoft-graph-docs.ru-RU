---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4aab80a23b72b599df7627f5734d04ad9aef0bbe
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2020
ms.locfileid: "44790938"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="e2eb6-104">Тип ресурса Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="e2eb6-104">educationSynchronizationCustomization resource type</span></span>

<span data-ttu-id="e2eb6-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2eb6-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2eb6-106">Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="e2eb6-106">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="e2eb6-107">Настройку можно применить ко всем синхронизированным сущностям.</span><span class="sxs-lookup"><span data-stu-id="e2eb6-107">The customization can be applied to all the entities being synchronized.</span></span>

## <a name="properties"></a><span data-ttu-id="e2eb6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e2eb6-108">Properties</span></span>

| <span data-ttu-id="e2eb6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e2eb6-109">Property</span></span>                 | <span data-ttu-id="e2eb6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e2eb6-110">Type</span></span>              | <span data-ttu-id="e2eb6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e2eb6-111">Description</span></span>                                                                                                                                                                                                            |
| :----------------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="e2eb6-112">оптионалпропертиестосинк</span><span class="sxs-lookup"><span data-stu-id="e2eb6-112">optionalPropertiesToSync</span></span> | <span data-ttu-id="e2eb6-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e2eb6-113">String collection</span></span> | <span data-ttu-id="e2eb6-114">Коллекция имен свойств, которые необходимо синхронизировать. Если задано значение null, все свойства будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="e2eb6-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span> <span data-ttu-id="e2eb6-115">**Не относится к регистрациям студентов или спискам преподавателей**</span><span class="sxs-lookup"><span data-stu-id="e2eb6-115">**Does not apply to Student Enrollments or Teacher Rosters**</span></span>                                                            |
| <span data-ttu-id="e2eb6-116">синчронизатионстартдате</span><span class="sxs-lookup"><span data-stu-id="e2eb6-116">synchronizationStartDate</span></span> | <span data-ttu-id="e2eb6-117">DateTime</span><span class="sxs-lookup"><span data-stu-id="e2eb6-117">DateTime</span></span>          | <span data-ttu-id="e2eb6-118">Дата начала синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e2eb6-118">The date that the synchronization should start.</span></span> <span data-ttu-id="e2eb6-119">Это значение должно быть равно дате в будущем.</span><span class="sxs-lookup"><span data-stu-id="e2eb6-119">This value should be set to a future date.</span></span> <span data-ttu-id="e2eb6-120">Если задано значение null, то при завершении настройки профиля ресурс будет синхронизирован.</span><span class="sxs-lookup"><span data-stu-id="e2eb6-120">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="e2eb6-121">**Применимо только к регистрациям для студентов**</span><span class="sxs-lookup"><span data-stu-id="e2eb6-121">**Only applies to Student Enrollments**</span></span> |
| <span data-ttu-id="e2eb6-122">иссинкдеферред</span><span class="sxs-lookup"><span data-stu-id="e2eb6-122">isSyncDeferred</span></span>           | <span data-ttu-id="e2eb6-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2eb6-123">Boolean</span></span>           | <span data-ttu-id="e2eb6-124">Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="e2eb6-124">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span>                                                                                                                                    |
| <span data-ttu-id="e2eb6-125">алловдисплайнамеупдате</span><span class="sxs-lookup"><span data-stu-id="e2eb6-125">allowDisplayNameUpdate</span></span>   | <span data-ttu-id="e2eb6-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="e2eb6-126">Boolean</span></span>           | <span data-ttu-id="e2eb6-127">Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.</span><span class="sxs-lookup"><span data-stu-id="e2eb6-127">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="e2eb6-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e2eb6-128">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationCustomization"
}-->

```json
{
  "optionalPropertiesToSync": ["String"],
  "synchronizationStartDate": "DateTimeOffset",
  "isSyncDeferred": "Boolean",
  "allowDisplayNameUpdate": "Boolean"
}
```
