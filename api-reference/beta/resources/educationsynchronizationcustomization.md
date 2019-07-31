---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 46cd20bbe016110a313d5b195a518ef81ca05afe
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972455"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="55741-104">Тип ресурса Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="55741-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55741-105">Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="55741-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="55741-106">Настройку можно применить ко всем синхронизированным сущностям.</span><span class="sxs-lookup"><span data-stu-id="55741-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="55741-107">**Примечание:** Свойство **синчронизатионстартдате** применяется только к объекту **студентенроллмент** .</span><span class="sxs-lookup"><span data-stu-id="55741-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="55741-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="55741-108">Properties</span></span>

| <span data-ttu-id="55741-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="55741-109">Property</span></span> | <span data-ttu-id="55741-110">Тип</span><span class="sxs-lookup"><span data-stu-id="55741-110">Type</span></span> | <span data-ttu-id="55741-111">Описание</span><span class="sxs-lookup"><span data-stu-id="55741-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="55741-112">**Оптионалпропертиестосинк**</span><span class="sxs-lookup"><span data-stu-id="55741-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="55741-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="55741-113">collection of string</span></span> |  <span data-ttu-id="55741-114">Коллекция имен свойств, которые необходимо синхронизировать. Если задано значение null, все свойства будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="55741-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="55741-115">**Синчронизатионстартдате**</span><span class="sxs-lookup"><span data-stu-id="55741-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="55741-116">DateTime</span><span class="sxs-lookup"><span data-stu-id="55741-116">DateTime</span></span> |  <span data-ttu-id="55741-117">Дата начала синхронизации.</span><span class="sxs-lookup"><span data-stu-id="55741-117">The date that the synchronization should start.</span></span> <span data-ttu-id="55741-118">Это значение должно быть равно дате в будущем.</span><span class="sxs-lookup"><span data-stu-id="55741-118">This value should be set to a future date.</span></span> <span data-ttu-id="55741-119">Если задано значение null, то при завершении настройки профиля ресурс будет синхронизирован.</span><span class="sxs-lookup"><span data-stu-id="55741-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="55741-120">**Примечание:** Это относится только к свойству **студентенроллмент** .</span><span class="sxs-lookup"><span data-stu-id="55741-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="55741-121">**Иссинкдеферред**</span><span class="sxs-lookup"><span data-stu-id="55741-121">**isSyncDeferred**</span></span> |<span data-ttu-id="55741-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="55741-122">Boolean</span></span> | <span data-ttu-id="55741-123">Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="55741-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="55741-124">**Алловдисплайнамеупдате**</span><span class="sxs-lookup"><span data-stu-id="55741-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="55741-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="55741-125">Boolean</span></span> |  <span data-ttu-id="55741-126">Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.</span><span class="sxs-lookup"><span data-stu-id="55741-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="55741-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="55741-127">JSON representation</span></span>
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
