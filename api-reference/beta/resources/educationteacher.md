---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4cd8b11d5f398177ec301e6cb7d834268e97c005
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909710"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="766bc-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="766bc-103">educationTeacher resource type</span></span>

<span data-ttu-id="766bc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="766bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="766bc-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="766bc-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="766bc-106">При использовании делегированных областей разрешений Graph будет возвращать только `externalId` Свойства.</span><span class="sxs-lookup"><span data-stu-id="766bc-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="766bc-107">Для всех остальных свойств требуются области применения.</span><span class="sxs-lookup"><span data-stu-id="766bc-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="766bc-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="766bc-108">Properties</span></span>

| <span data-ttu-id="766bc-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="766bc-109">Property</span></span>      | <span data-ttu-id="766bc-110">Тип</span><span class="sxs-lookup"><span data-stu-id="766bc-110">Type</span></span>   | <span data-ttu-id="766bc-111">Описание</span><span class="sxs-lookup"><span data-stu-id="766bc-111">Description</span></span>                                  |
| :------------ | :----- | :------------------------------------------- |
| <span data-ttu-id="766bc-112">externalId</span><span class="sxs-lookup"><span data-stu-id="766bc-112">externalId</span></span>    | <span data-ttu-id="766bc-113">String</span><span class="sxs-lookup"><span data-stu-id="766bc-113">String</span></span> | <span data-ttu-id="766bc-114">Идентификатор преподавателя во внешней исходной системе.</span><span class="sxs-lookup"><span data-stu-id="766bc-114">Id of the Teacher in external source system.</span></span> |
| <span data-ttu-id="766bc-115">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="766bc-115">teacherNumber</span></span> | <span data-ttu-id="766bc-116">String</span><span class="sxs-lookup"><span data-stu-id="766bc-116">String</span></span> | <span data-ttu-id="766bc-117">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="766bc-117">Teacher number.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="766bc-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="766bc-118">JSON representation</span></span>

<span data-ttu-id="766bc-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="766bc-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTeacher"
}-->

```json
{
  "externalId": "String",
  "teacherNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTeacher resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
