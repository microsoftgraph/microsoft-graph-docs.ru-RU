---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 6e5e60f04af74cd09f893823e9544ba455b60113
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231845"
---
# <a name="teacher-resource-type"></a><span data-ttu-id="c538d-103">Тип ресурса Teacher</span><span class="sxs-lookup"><span data-stu-id="c538d-103">Teacher resource type</span></span>

<span data-ttu-id="c538d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c538d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c538d-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="c538d-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>

## <a name="properties"></a><span data-ttu-id="c538d-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c538d-106">Properties</span></span>

| <span data-ttu-id="c538d-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c538d-107">Property</span></span>      | <span data-ttu-id="c538d-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c538d-108">Type</span></span>   | <span data-ttu-id="c538d-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c538d-109">Description</span></span>                             |
| :------------ | :----- | :-------------------------------------- |
| <span data-ttu-id="c538d-110">externalId</span><span class="sxs-lookup"><span data-stu-id="c538d-110">externalId</span></span>    | <span data-ttu-id="c538d-111">String</span><span class="sxs-lookup"><span data-stu-id="c538d-111">String</span></span> | <span data-ttu-id="c538d-112">Идентификатор преподавателя в исходной системе.</span><span class="sxs-lookup"><span data-stu-id="c538d-112">ID of the teacher in the source system.</span></span> |
| <span data-ttu-id="c538d-113">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="c538d-113">teacherNumber</span></span> | <span data-ttu-id="c538d-114">String</span><span class="sxs-lookup"><span data-stu-id="c538d-114">String</span></span> | <span data-ttu-id="c538d-115">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="c538d-115">Teacher number.</span></span>                         |

## <a name="relationships"></a><span data-ttu-id="c538d-116">Связи</span><span class="sxs-lookup"><span data-stu-id="c538d-116">Relationships</span></span>

<span data-ttu-id="c538d-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c538d-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c538d-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c538d-118">JSON representation</span></span>

<span data-ttu-id="c538d-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c538d-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationTeacher"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationTeacher",
  "teacherNumber": "String",
  "externalId": "String"
}
```
