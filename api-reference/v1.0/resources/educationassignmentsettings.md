---
title: тип ресурса educationAssignmentSettings
description: Указывает параметры назначений на уровне класса.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ccaa51c84e50e2f9c5302836ffd9b92754f517fd
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912937"
---
# <a name="educationassignmentsettings-resource-type"></a><span data-ttu-id="83b19-103">тип ресурса educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="83b19-103">educationAssignmentSettings resource type</span></span>

<span data-ttu-id="83b19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83b19-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83b19-105">Указывает параметры назначений на уровне класса.</span><span class="sxs-lookup"><span data-stu-id="83b19-105">Specifies class-level assignments settings.</span></span>

## <a name="methods"></a><span data-ttu-id="83b19-106">Методы</span><span class="sxs-lookup"><span data-stu-id="83b19-106">Methods</span></span>
|<span data-ttu-id="83b19-107">Метод</span><span class="sxs-lookup"><span data-stu-id="83b19-107">Method</span></span>|<span data-ttu-id="83b19-108">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="83b19-108">Return type</span></span>|<span data-ttu-id="83b19-109">Описание</span><span class="sxs-lookup"><span data-stu-id="83b19-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="83b19-110">Get educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="83b19-110">Get educationAssignmentSettings</span></span>](../api/educationassignmentsettings-get.md)|[<span data-ttu-id="83b19-111">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="83b19-111">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="83b19-112">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="83b19-112">Read the properties and relationships of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|
|[<span data-ttu-id="83b19-113">Обновление educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="83b19-113">Update educationAssignmentSettings</span></span>](../api/educationassignmentsettings-update.md)|[<span data-ttu-id="83b19-114">educationAssignmentSettings</span><span class="sxs-lookup"><span data-stu-id="83b19-114">educationAssignmentSettings</span></span>](../resources/educationassignmentsettings.md)|<span data-ttu-id="83b19-115">Обновление свойств объекта [educationAssignmentSettings.](../resources/educationassignmentsettings.md)</span><span class="sxs-lookup"><span data-stu-id="83b19-115">Update the properties of an [educationAssignmentSettings](../resources/educationassignmentsettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="83b19-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="83b19-116">Properties</span></span>
|<span data-ttu-id="83b19-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="83b19-117">Property</span></span>|<span data-ttu-id="83b19-118">Тип</span><span class="sxs-lookup"><span data-stu-id="83b19-118">Type</span></span>|<span data-ttu-id="83b19-119">Описание</span><span class="sxs-lookup"><span data-stu-id="83b19-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83b19-120">submissionAnimationDisabled</span><span class="sxs-lookup"><span data-stu-id="83b19-120">submissionAnimationDisabled</span></span>|<span data-ttu-id="83b19-121">Логический</span><span class="sxs-lookup"><span data-stu-id="83b19-121">Boolean</span></span>|<span data-ttu-id="83b19-122">Указывает, будет ли показана анимация празднования по очереди.</span><span class="sxs-lookup"><span data-stu-id="83b19-122">Indicates whether turn-in celebration animation will be shown.</span></span> <span data-ttu-id="83b19-123">Значение `true` указывает, что анимация не будет показана.</span><span class="sxs-lookup"><span data-stu-id="83b19-123">A value of `true` indicates that the animation will not be shown.</span></span> <span data-ttu-id="83b19-124">Значение по умолчанию — `false`.</span><span class="sxs-lookup"><span data-stu-id="83b19-124">Default value is `false`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="83b19-125">Связи</span><span class="sxs-lookup"><span data-stu-id="83b19-125">Relationships</span></span>
<span data-ttu-id="83b19-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="83b19-126">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="83b19-127">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="83b19-127">JSON representation</span></span>
<span data-ttu-id="83b19-128">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="83b19-128">The following is a JSON representation of the resource.</span></span>
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

