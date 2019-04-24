---
title: Тип ресурса Едукатионсинчронизатионкустомизатион
description: 'Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов. Настройку можно применить ко всем синхронизированным сущностям. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 8af6c5e2173a8b04e730529123b4608fd236f959
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507054"
---
# <a name="educationsynchronizationcustomization-resource-type"></a><span data-ttu-id="d5388-104">Тип ресурса Едукатионсинчронизатионкустомизатион</span><span class="sxs-lookup"><span data-stu-id="d5388-104">educationSynchronizationCustomization resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5388-105">Предоставляет параметры для настройки синхронизации профилей данных School для сущностей ресурсов.</span><span class="sxs-lookup"><span data-stu-id="d5388-105">Provides settings for customizing the school data profile synchronization of the resource entities.</span></span> <span data-ttu-id="d5388-106">Настройку можно применить ко всем синхронизированным сущностям.</span><span class="sxs-lookup"><span data-stu-id="d5388-106">The customization can be applied to all the entities being synchronized.</span></span> 

><span data-ttu-id="d5388-107">**Примечание:** Свойство **синчронизатионстартдате** применяется только к объекту **студентенроллмент** .</span><span class="sxs-lookup"><span data-stu-id="d5388-107">**Note:** The **synchronizationStartDate** property only applies to the **StudentEnrollment** entity.</span></span>

## <a name="properties"></a><span data-ttu-id="d5388-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d5388-108">Properties</span></span>

| <span data-ttu-id="d5388-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d5388-109">Property</span></span> | <span data-ttu-id="d5388-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d5388-110">Type</span></span> | <span data-ttu-id="d5388-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d5388-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="d5388-112">**Оптионалпропертиестосинк**</span><span class="sxs-lookup"><span data-stu-id="d5388-112">**optionalPropertiesToSync**</span></span> | <span data-ttu-id="d5388-113">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="d5388-113">collection of string</span></span> |  <span data-ttu-id="d5388-114">Коллекция имен свойств, которые необходимо синхронизировать. Если задано значение null, все свойства будут синхронизированы.</span><span class="sxs-lookup"><span data-stu-id="d5388-114">The collection of property names to sync. If set to null, all properties will be synchronized.</span></span>       |
| <span data-ttu-id="d5388-115">**Синчронизатионстартдате**</span><span class="sxs-lookup"><span data-stu-id="d5388-115">**synchronizationStartDate**</span></span> | <span data-ttu-id="d5388-116">DateTime</span><span class="sxs-lookup"><span data-stu-id="d5388-116">DateTime</span></span> |  <span data-ttu-id="d5388-117">Дата начала синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d5388-117">The date that the synchronization should start.</span></span> <span data-ttu-id="d5388-118">Это значение должно быть равно дате в будущем.</span><span class="sxs-lookup"><span data-stu-id="d5388-118">This value should be set to a future date.</span></span> <span data-ttu-id="d5388-119">Если задано значение null, то при завершении настройки профиля ресурс будет синхронизирован.</span><span class="sxs-lookup"><span data-stu-id="d5388-119">If set to null, the resource will be synchronized when the profile setup completes.</span></span> <span data-ttu-id="d5388-120">**Примечание:** Это относится только к свойству **студентенроллмент** .</span><span class="sxs-lookup"><span data-stu-id="d5388-120">**Note:** This only applies to the **StudentEnrollment** property.</span></span>      |
|<span data-ttu-id="d5388-121">**Иссинкдеферред**</span><span class="sxs-lookup"><span data-stu-id="d5388-121">**isSyncDeferred**</span></span> |<span data-ttu-id="d5388-122">Логический</span><span class="sxs-lookup"><span data-stu-id="d5388-122">Boolean</span></span> | <span data-ttu-id="d5388-123">Указывает, откладывается ли синхронизация родительской сущности на более позднюю дату.</span><span class="sxs-lookup"><span data-stu-id="d5388-123">Indicates whether synchronization of the parent entity is deferred to a later date.</span></span> |
| <span data-ttu-id="d5388-124">**Алловдисплайнамеупдате**</span><span class="sxs-lookup"><span data-stu-id="d5388-124">**allowDisplayNameUpdate**</span></span> | <span data-ttu-id="d5388-125">Логический</span><span class="sxs-lookup"><span data-stu-id="d5388-125">Boolean</span></span> |  <span data-ttu-id="d5388-126">Указывает, может ли отображаемое имя ресурса быть перезаписано при синхронизации.</span><span class="sxs-lookup"><span data-stu-id="d5388-126">Indicates whether the display name of the resource can be overwritten by the sync.</span></span>         |


## <a name="json-representation"></a><span data-ttu-id="d5388-127">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d5388-127">JSON representation</span></span>
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
