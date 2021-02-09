---
title: Тип ресурса educationAssignmentSettings
description: Указывает параметры назначений на уровне класса.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d5990453eefbe63013ecfa0be03ff5b4d99330fa
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153655"
---
# <a name="educationassignmentsettings-resource-type"></a><span data-ttu-id="980d2-103">Тип ресурса educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="980d2-103">educationAssignmentSettings resource type</span></span>

<span data-ttu-id="980d2-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="980d2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="980d2-105">Указывает параметры назначений на уровне класса.</span><span class="sxs-lookup"><span data-stu-id="980d2-105">Specifies class-level assignments settings.</span></span>

## <a name="methods"></a><span data-ttu-id="980d2-106">Методы</span><span class="sxs-lookup"><span data-stu-id="980d2-106">Methods</span></span>
|<span data-ttu-id="980d2-107">Метод</span><span class="sxs-lookup"><span data-stu-id="980d2-107">Method</span></span>|<span data-ttu-id="980d2-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="980d2-108">Return type</span></span>|<span data-ttu-id="980d2-109">Описание</span><span class="sxs-lookup"><span data-stu-id="980d2-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="980d2-110">Get educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="980d2-110">Get educationAssignmentSettings</span></span>](../api/educationassignmentsettings-get.md)|[<span data-ttu-id="980d2-111">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="980d2-111">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="980d2-112">Чтение свойств и связей объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="980d2-112">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|
|[<span data-ttu-id="980d2-113">Обновление educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="980d2-113">Update educationAssignmentSettings</span></span>](../api/educationassignmentsettings-update.md)|[<span data-ttu-id="980d2-114">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="980d2-114">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="980d2-115">Обновление свойств объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="980d2-115">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="980d2-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="980d2-116">Properties</span></span>
|<span data-ttu-id="980d2-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="980d2-117">Property</span></span>|<span data-ttu-id="980d2-118">Тип</span><span class="sxs-lookup"><span data-stu-id="980d2-118">Type</span></span>|<span data-ttu-id="980d2-119">Описание</span><span class="sxs-lookup"><span data-stu-id="980d2-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="980d2-120">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="980d2-120">submissionAnimationDisabled</span></span>|<span data-ttu-id="980d2-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="980d2-121">Boolean</span></span>|<span data-ttu-id="980d2-122">Указывает, будет ли показана анимация поозднения.</span><span class="sxs-lookup"><span data-stu-id="980d2-122">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="980d2-123">Значение `true` указывает, что анимация не будет показана.</span><span class="sxs-lookup"><span data-stu-id="980d2-123">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="980d2-124">Значение по умолчанию: `false`.</span><span class="sxs-lookup"><span data-stu-id="980d2-124">Default value is `false`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="980d2-125">Связи</span><span class="sxs-lookup"><span data-stu-id="980d2-125">Relationships</span></span>
<span data-ttu-id="980d2-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="980d2-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="980d2-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="980d2-127">JSON representation</span></span>
<span data-ttu-id="980d2-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="980d2-128">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentSettings",
  "openType": false
}
-->
``` json
{
  "submissionAnimationDisabled": false
}
```

