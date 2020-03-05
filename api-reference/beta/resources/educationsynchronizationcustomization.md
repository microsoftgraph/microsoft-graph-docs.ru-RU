---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 368117a5293f4ede59282fa1ced12d024976de52
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500466"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="a7059-104">Тип ресурса Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="a7059-104">educationSynchronizationCustomization resource type</span></span>

<span data-ttu-id="a7059-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a7059-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7059-106">Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="a7059-106">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="a7059-107">Настройку можно применить ко всем синхронизированным сущностям.</span><span class="sxs-lookup"><span data-stu-id="a7059-107">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="a7059-108">**Примечание:** Свойство **синчронизатионстартдате** применяется только к объекту **студентенроллмент** .</span><span class="sxs-lookup"><span data-stu-id="a7059-108">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="a7059-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7059-109">Properties</span></span>

| <span data-ttu-id="a7059-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7059-110">Property</span></span> | <span data-ttu-id="a7059-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a7059-111">Type</span></span> | <span data-ttu-id="a7059-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a7059-112">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a7059-113">**оптионалпропертиестосинк**</span><span class="sxs-lookup"><span data-stu-id="a7059-113">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="a7059-114">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="a7059-114">collection of string</span></span> |  <span data-ttu-id="a7059-115">Коллекция имен свойств, которые необходимо синхронизировать. Если задано значение null, все свойства будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="a7059-115">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="a7059-116">**синчронизатионстартдате**</span><span class="sxs-lookup"><span data-stu-id="a7059-116">**synchronizationStartDate**</span></span> | <span data-ttu-id="a7059-117">DateTime</span><span class="sxs-lookup"><span data-stu-id="a7059-117">DateTime</span></span> |  <span data-ttu-id="a7059-118">Дата начала синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a7059-118">The date that the synchronization should start.</span></span> <span data-ttu-id="a7059-119">Это значение должно быть равно дате в будущем.</span><span class="sxs-lookup"><span data-stu-id="a7059-119">This value should be set to a future date.</span></span> <span data-ttu-id="a7059-120">Если задано значение null, то при завершении настройки профиля ресурс будет синхронизирован.</span><span class="sxs-lookup"><span data-stu-id="a7059-120">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="a7059-121">**Примечание:** Это относится только к свойству **студентенроллмент** .</span><span class="sxs-lookup"><span data-stu-id="a7059-121">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="a7059-122">**иссинкдеферред**</span><span class="sxs-lookup"><span data-stu-id="a7059-122">**isSyncDeferred**</span></span> |<span data-ttu-id="a7059-123">Логический</span><span class="sxs-lookup"><span data-stu-id="a7059-123">Boolean</span></span> | <span data-ttu-id="a7059-124">Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="a7059-124">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="a7059-125">**алловдисплайнамеупдате**</span><span class="sxs-lookup"><span data-stu-id="a7059-125">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="a7059-126">Логический</span><span class="sxs-lookup"><span data-stu-id="a7059-126">Boolean</span></span> |  <span data-ttu-id="a7059-127">Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.</span><span class="sxs-lookup"><span data-stu-id="a7059-127">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="a7059-128">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7059-128">JSON representation</span></span>
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
