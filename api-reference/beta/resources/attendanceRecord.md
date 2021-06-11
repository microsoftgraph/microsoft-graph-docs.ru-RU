---
title: тип ресурса attendanceRecord
description: Содержит сведения, связанные с записью посещаемости в отчете о посещаемости собрания.
author: mkhribech
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 20beeca97c790b8743c9038e7fddf0b5c6f69534
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896503"
---
# <a name="attendancerecord-resource-type"></a><span data-ttu-id="31de1-103">тип ресурса attendanceRecord</span><span class="sxs-lookup"><span data-stu-id="31de1-103">attendanceRecord resource type</span></span>

<span data-ttu-id="31de1-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="31de1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31de1-105">Содержит сведения, связанные с записью посещаемости в отчете о посещаемости собрания.</span><span class="sxs-lookup"><span data-stu-id="31de1-105">Contains information associated with attendance record in meeting attendance report.</span></span>

## <a name="properties"></a><span data-ttu-id="31de1-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="31de1-106">Properties</span></span>

| <span data-ttu-id="31de1-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="31de1-107">Property</span></span>            | <span data-ttu-id="31de1-108">Тип</span><span class="sxs-lookup"><span data-stu-id="31de1-108">Type</span></span>    | <span data-ttu-id="31de1-109">Описание</span><span class="sxs-lookup"><span data-stu-id="31de1-109">Description</span></span>|
|:--------------------|:--------|:-----------|
| <span data-ttu-id="31de1-110">удостоверение</span><span class="sxs-lookup"><span data-stu-id="31de1-110">identity</span></span> | [<span data-ttu-id="31de1-111">Identity</span><span class="sxs-lookup"><span data-stu-id="31de1-111">Identity</span></span>](identity.md) | <span data-ttu-id="31de1-112">Идентификатор, например имя отображения.</span><span class="sxs-lookup"><span data-stu-id="31de1-112">Identifier, such as display name.</span></span> |
| <span data-ttu-id="31de1-113">emailAddress</span><span class="sxs-lookup"><span data-stu-id="31de1-113">emailAddress</span></span> | <span data-ttu-id="31de1-114">String</span><span class="sxs-lookup"><span data-stu-id="31de1-114">String</span></span> | <span data-ttu-id="31de1-115">Адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="31de1-115">Email address.</span></span> |
| <span data-ttu-id="31de1-116">totalAttendanceInSeconds</span><span class="sxs-lookup"><span data-stu-id="31de1-116">totalAttendanceInSeconds</span></span> | <span data-ttu-id="31de1-117">Int32</span><span class="sxs-lookup"><span data-stu-id="31de1-117">Int32</span></span> | <span data-ttu-id="31de1-118">Общая продолжительность посещаемости в секундах.</span><span class="sxs-lookup"><span data-stu-id="31de1-118">Total duration of the attendances in seconds.</span></span> |
| <span data-ttu-id="31de1-119">attendanceIntervals</span><span class="sxs-lookup"><span data-stu-id="31de1-119">attendanceIntervals</span></span> | <span data-ttu-id="31de1-120">[коллекция attendanceInterval](attendanceInterval.md)</span><span class="sxs-lookup"><span data-stu-id="31de1-120">[attendanceInterval](attendanceInterval.md) collection</span></span> | <span data-ttu-id="31de1-121">Список периодов времени между присоединением и отъездом.</span><span class="sxs-lookup"><span data-stu-id="31de1-121">List of time periods between joining and leaving.</span></span> |
| <span data-ttu-id="31de1-122">role</span><span class="sxs-lookup"><span data-stu-id="31de1-122">role</span></span> | <span data-ttu-id="31de1-123">String</span><span class="sxs-lookup"><span data-stu-id="31de1-123">String</span></span> | <span data-ttu-id="31de1-124">Роль участника.</span><span class="sxs-lookup"><span data-stu-id="31de1-124">Role of the attendee.</span></span> <span data-ttu-id="31de1-125">Возможные значения `None` , `Attendee` и `Presenter` `Organizer` .</span><span class="sxs-lookup"><span data-stu-id="31de1-125">Possible values are `None`, `Attendee`, `Presenter`, and `Organizer`.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="31de1-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="31de1-126">JSON representation</span></span>

<span data-ttu-id="31de1-127">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="31de1-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.attendanceRecord"
}-->

```json

{
    "emailAddress": "String",
    "totalAttendanceInSeconds": "Int32",
    "role": "String(None|Attendee|Presenter|Organizer)",
    "identity": {"@odata.type": "#microsoft.graph.identity"},
    "attendanceIntervals": [{"@odata.type": "#microsoft.graph.attendanceInterval"}]
}

```
