---
title: тип ресурса educationAssignmentDefaults
description: Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе.
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cdd4cb3814900f41f7cb7ee5ede407af61e9c4d7
ms.sourcegitcommit: 3f40fbb953b14c1f52341786569c678adfc5bd3e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/05/2021
ms.locfileid: "52781067"
---
# <a name="educationassignmentdefaults-resource-type"></a><span data-ttu-id="9c326-103">тип ресурса educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="9c326-103">educationAssignmentDefaults resource type</span></span>

<span data-ttu-id="9c326-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9c326-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c326-105">Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе.</span><span class="sxs-lookup"><span data-stu-id="9c326-105">Specifies class-level defaults respected by new assignments created in the class.</span></span> <span data-ttu-id="9c326-106">Звонители могут продолжать указывать настраиваемые значения для каждого создания назначения, если они не хотят поведения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="9c326-106">Callers can continue to specify custom values on each assignment creation if they do not want the default behaviors.</span></span>

## <a name="methods"></a><span data-ttu-id="9c326-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9c326-107">Methods</span></span>
|<span data-ttu-id="9c326-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9c326-108">Method</span></span>|<span data-ttu-id="9c326-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="9c326-109">Return type</span></span>|<span data-ttu-id="9c326-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9c326-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9c326-111">Get educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="9c326-111">Get educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-get.md)|[<span data-ttu-id="9c326-112">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="9c326-112">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="9c326-113">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="9c326-113">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|
|[<span data-ttu-id="9c326-114">Обновление educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="9c326-114">Update educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-update.md)|[<span data-ttu-id="9c326-115">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="9c326-115">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="9c326-116">Обновление свойств объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="9c326-116">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c326-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="9c326-117">Properties</span></span>
|<span data-ttu-id="9c326-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="9c326-118">Property</span></span>|<span data-ttu-id="9c326-119">Тип</span><span class="sxs-lookup"><span data-stu-id="9c326-119">Type</span></span>|<span data-ttu-id="9c326-120">Описание</span><span class="sxs-lookup"><span data-stu-id="9c326-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c326-121">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="9c326-121">addedStudentAction</span></span>|<span data-ttu-id="9c326-122">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="9c326-122">educationAddedStudentAction</span></span>|<span data-ttu-id="9c326-123">Поведение по умолчанию на уровне класса для обработки учащихся, добавленных после публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="9c326-123">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="9c326-124">Возможные значения: `none`, `assignIfOpen`.</span><span class="sxs-lookup"><span data-stu-id="9c326-124">Possible values are: `none`, `assignIfOpen`.</span></span>|
|<span data-ttu-id="9c326-125">addToCalendarAction</span><span class="sxs-lookup"><span data-stu-id="9c326-125">addToCalendarAction</span></span>| <span data-ttu-id="9c326-126">educationAddToCalendarOptions</span><span class="sxs-lookup"><span data-stu-id="9c326-126">educationAddToCalendarOptions</span></span>|<span data-ttu-id="9c326-127">Необязательное поле для управления asfor добавлением назначений в календари учащихся и преподавателей при публикации задания.</span><span class="sxs-lookup"><span data-stu-id="9c326-127">Optional field to control the asfor adding assignments to students' and teachers' calendars when the assignment is published.</span></span> <span data-ttu-id="9c326-128">Возможные значения: `studentsAndPublisher`, `studentsAndTeamOwners`, `none`.</span><span class="sxs-lookup"><span data-stu-id="9c326-128">Possible values are: `studentsAndPublisher`, `studentsAndTeamOwners`, `none`.</span></span> <span data-ttu-id="9c326-129">Значение по умолчанию — `none`.</span><span class="sxs-lookup"><span data-stu-id="9c326-129">Default value is `none`.</span></span>|
|<span data-ttu-id="9c326-130">dueTime</span><span class="sxs-lookup"><span data-stu-id="9c326-130">dueTime</span></span>|<span data-ttu-id="9c326-131">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="9c326-131">TimeOfDay</span></span>|<span data-ttu-id="9c326-132">Значение по умолчанию класса для должного поля времени.</span><span class="sxs-lookup"><span data-stu-id="9c326-132">Class-level default value for due time field.</span></span> <span data-ttu-id="9c326-133">Значение по умолчанию — `23:59:00`.</span><span class="sxs-lookup"><span data-stu-id="9c326-133">Default value is `23:59:00`.</span></span>|
|<span data-ttu-id="9c326-134">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="9c326-134">notificationChannelUrl</span></span>|<span data-ttu-id="9c326-135">String</span><span class="sxs-lookup"><span data-stu-id="9c326-135">String</span></span>|<span data-ttu-id="9c326-136">По умолчанию Teams канал, в который будут отправлены уведомления.</span><span class="sxs-lookup"><span data-stu-id="9c326-136">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="9c326-137">Значение по умолчанию — `null`.</span><span class="sxs-lookup"><span data-stu-id="9c326-137">Default value is `null`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9c326-138">Связи</span><span class="sxs-lookup"><span data-stu-id="9c326-138">Relationships</span></span>
<span data-ttu-id="9c326-139">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9c326-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c326-140">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9c326-140">JSON representation</span></span>
<span data-ttu-id="9c326-141">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9c326-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "addedStudentAction": "none",
  "addToCalendarAction": "none",
  "dueTime": "23:59:00",
  "notificationChannelUrl": "https://graph.microsoft.com/beta/teams('id')/channels('id')"
}
```

