---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c3f704339dbf2acbe7cb78e1899c5f209f50f21e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055596"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="12faa-104">Тип ресурса Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="12faa-104">educationSynchronizationCustomization resource type</span></span>

<span data-ttu-id="12faa-105">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12faa-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12faa-106">Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="12faa-106">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="12faa-107">Настройку можно применить ко всем синхронизированным сущностям.</span><span class="sxs-lookup"><span data-stu-id="12faa-107">The customization can be applied to all the entities being synchronized.</span></span>

## <a name="properties"></a><span data-ttu-id="12faa-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="12faa-108">Properties</span></span>

| <span data-ttu-id="12faa-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="12faa-109">Property</span></span>                 | <span data-ttu-id="12faa-110">Тип</span><span class="sxs-lookup"><span data-stu-id="12faa-110">Type</span></span>              | <span data-ttu-id="12faa-111">Описание</span><span class="sxs-lookup"><span data-stu-id="12faa-111">Description</span></span>                                                                                                                                                                                                            |
| :----------------------- | :---------------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="12faa-112">оптионалпропертиестосинк</span><span class="sxs-lookup"><span data-stu-id="12faa-112">optionalPropertiesToSync</span></span> | <span data-ttu-id="12faa-113">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="12faa-113">String collection</span></span> | <span data-ttu-id="12faa-114">Коллекция имен свойств, которые необходимо синхронизировать. Если задано значение null, все свойства будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="12faa-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span> <span data-ttu-id="12faa-115">**Не относится к регистрациям студентов или спискам преподавателей**</span><span class="sxs-lookup"><span data-stu-id="12faa-115">**Does not apply to Student Enrollments or Teacher Rosters**</span></span>                                                            |
| <span data-ttu-id="12faa-116">синчронизатионстартдате</span><span class="sxs-lookup"><span data-stu-id="12faa-116">synchronizationStartDate</span></span> | <span data-ttu-id="12faa-117">DateTime</span><span class="sxs-lookup"><span data-stu-id="12faa-117">DateTime</span></span>          | <span data-ttu-id="12faa-118">Дата начала синхронизации.</span><span class="sxs-lookup"><span data-stu-id="12faa-118">The date that the synchronization should start.</span></span> <span data-ttu-id="12faa-119">Это значение должно быть равно дате в будущем.</span><span class="sxs-lookup"><span data-stu-id="12faa-119">This value should be set to a future date.</span></span> <span data-ttu-id="12faa-120">Если задано значение null, то при завершении настройки профиля ресурс будет синхронизирован.</span><span class="sxs-lookup"><span data-stu-id="12faa-120">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="12faa-121">**Применимо только к регистрациям для студентов**</span><span class="sxs-lookup"><span data-stu-id="12faa-121">**Only applies to Student Enrollments**</span></span> |
| <span data-ttu-id="12faa-122">иссинкдеферред</span><span class="sxs-lookup"><span data-stu-id="12faa-122">isSyncDeferred</span></span>           | <span data-ttu-id="12faa-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="12faa-123">Boolean</span></span>           | <span data-ttu-id="12faa-124">Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="12faa-124">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span>                                                                                                                                    |
| <span data-ttu-id="12faa-125">алловдисплайнамеупдате</span><span class="sxs-lookup"><span data-stu-id="12faa-125">allowDisplayNameUpdate</span></span>   | <span data-ttu-id="12faa-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="12faa-126">Boolean</span></span>           | <span data-ttu-id="12faa-127">Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.</span><span class="sxs-lookup"><span data-stu-id="12faa-127">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>                                                                                                                                     |

## <a name="json-representation"></a><span data-ttu-id="12faa-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="12faa-128">JSON representation</span></span>

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


