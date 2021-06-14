---
title: тип ресурса educationAssignmentDefaults
description: Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе.
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e990e7fe940fface9ecc33d066ce86b6cc331e4f
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912652"
---
# <a name="educationassignmentdefaults-resource-type"></a><span data-ttu-id="248ea-103">тип ресурса educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="248ea-103">educationAssignmentDefaults resource type</span></span>

<span data-ttu-id="248ea-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="248ea-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="248ea-105">Указывает по умолчанию класса, которые соблюдаются новыми назначениями, созданными в классе.</span><span class="sxs-lookup"><span data-stu-id="248ea-105">Specifies class-level defaults respected by new assignments created in the class.</span></span> 

<span data-ttu-id="248ea-106">Звонители могут продолжать указывать настраиваемые значения для каждого создания назначения, если они не хотят поведения по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="248ea-106">Callers can continue to specify custom values on each assignment creation if they Don't want the default behaviors.</span></span>

## <a name="methods"></a><span data-ttu-id="248ea-107">Методы</span><span class="sxs-lookup"><span data-stu-id="248ea-107">Methods</span></span>
|<span data-ttu-id="248ea-108">Метод</span><span class="sxs-lookup"><span data-stu-id="248ea-108">Method</span></span>|<span data-ttu-id="248ea-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="248ea-109">Return type</span></span>|<span data-ttu-id="248ea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="248ea-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="248ea-111">Get educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="248ea-111">Get educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-get.md)|[<span data-ttu-id="248ea-112">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="248ea-112">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="248ea-113">Ознакомьтесь с свойствами и отношениями объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="248ea-113">Read the properties and relationships of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|
|[<span data-ttu-id="248ea-114">Обновление educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="248ea-114">Update educationAssignmentDefaults</span></span>](../api/educationassignmentdefaults-update.md)|[<span data-ttu-id="248ea-115">educationAssignmentDefaults</span><span class="sxs-lookup"><span data-stu-id="248ea-115">educationAssignmentDefaults</span></span>](../resources/educationassignmentdefaults.md)|<span data-ttu-id="248ea-116">Обновление свойств объекта [educationAssignmentDefaults.](../resources/educationassignmentdefaults.md)</span><span class="sxs-lookup"><span data-stu-id="248ea-116">Update the properties of an [educationAssignmentDefaults](../resources/educationassignmentdefaults.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="248ea-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="248ea-117">Properties</span></span>
|<span data-ttu-id="248ea-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="248ea-118">Property</span></span>|<span data-ttu-id="248ea-119">Тип</span><span class="sxs-lookup"><span data-stu-id="248ea-119">Type</span></span>|<span data-ttu-id="248ea-120">Описание</span><span class="sxs-lookup"><span data-stu-id="248ea-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="248ea-121">addedStudentAction</span><span class="sxs-lookup"><span data-stu-id="248ea-121">addedStudentAction</span></span>|<span data-ttu-id="248ea-122">educationAddedStudentAction</span><span class="sxs-lookup"><span data-stu-id="248ea-122">educationAddedStudentAction</span></span>|<span data-ttu-id="248ea-123">Поведение по умолчанию на уровне класса для обработки учащихся, добавленных после публикации назначения.</span><span class="sxs-lookup"><span data-stu-id="248ea-123">Class-level default behavior for handling students who are added after the assignment is published.</span></span> <span data-ttu-id="248ea-124">Возможные значения: `none`, `assignIfOpen`.</span><span class="sxs-lookup"><span data-stu-id="248ea-124">Possible values are: `none`, `assignIfOpen`.</span></span>|
|<span data-ttu-id="248ea-125">dueTime</span><span class="sxs-lookup"><span data-stu-id="248ea-125">dueTime</span></span>|<span data-ttu-id="248ea-126">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="248ea-126">TimeOfDay</span></span>|<span data-ttu-id="248ea-127">Значение по умолчанию класса для должного поля времени.</span><span class="sxs-lookup"><span data-stu-id="248ea-127">Class-level default value for due time field.</span></span> <span data-ttu-id="248ea-128">Значение по умолчанию — `23:59:00`.</span><span class="sxs-lookup"><span data-stu-id="248ea-128">Default value is `23:59:00`.</span></span>|
|<span data-ttu-id="248ea-129">notificationChannelUrl</span><span class="sxs-lookup"><span data-stu-id="248ea-129">notificationChannelUrl</span></span>|<span data-ttu-id="248ea-130">String</span><span class="sxs-lookup"><span data-stu-id="248ea-130">String</span></span>|<span data-ttu-id="248ea-131">По умолчанию Teams канал, в который будут отправлены уведомления.</span><span class="sxs-lookup"><span data-stu-id="248ea-131">Default Teams channel to which notifications will be sent.</span></span> <span data-ttu-id="248ea-132">Значение по умолчанию — `null`.</span><span class="sxs-lookup"><span data-stu-id="248ea-132">Default value is `null`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="248ea-133">Связи</span><span class="sxs-lookup"><span data-stu-id="248ea-133">Relationships</span></span>
<span data-ttu-id="248ea-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="248ea-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="248ea-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="248ea-135">JSON representation</span></span>
<span data-ttu-id="248ea-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="248ea-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationAssignmentDefaults",
  "openType": false
}
-->
``` json
{
  "addedStudentAction": "String",
  "dueTime": "String (timestamp)",
  "notificationChannelUrl": "String"
}
```

