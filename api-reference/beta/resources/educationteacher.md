---
title: Тип ресурса educationTeacher
description: Дополнительные сведения, добавляемые в объект educationUser, который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a2eae690076553090dbd32f46f0b777a998b615d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47979541"
---
# <a name="educationteacher-resource-type"></a><span data-ttu-id="2a377-103">Тип ресурса educationTeacher</span><span class="sxs-lookup"><span data-stu-id="2a377-103">educationTeacher resource type</span></span>

<span data-ttu-id="2a377-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a377-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a377-105">Дополнительные сведения, добавляемые в объект [educationUser](educationuser.md), который присутствует, когда значение параметра primaryRole для пользователя — `teacher`.</span><span class="sxs-lookup"><span data-stu-id="2a377-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `teacher`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="2a377-106">При использовании делегированных областей разрешений Graph будет возвращать только `externalId` Свойства.</span><span class="sxs-lookup"><span data-stu-id="2a377-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="2a377-107">Для всех остальных свойств требуются области применения.</span><span class="sxs-lookup"><span data-stu-id="2a377-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="2a377-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="2a377-108">Properties</span></span>

| <span data-ttu-id="2a377-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="2a377-109">Property</span></span>      | <span data-ttu-id="2a377-110">Тип</span><span class="sxs-lookup"><span data-stu-id="2a377-110">Type</span></span>   | <span data-ttu-id="2a377-111">Описание</span><span class="sxs-lookup"><span data-stu-id="2a377-111">Description</span></span>                                  |
| :------------ | :----- | :------------------------------------------- |
| <span data-ttu-id="2a377-112">externalId</span><span class="sxs-lookup"><span data-stu-id="2a377-112">externalId</span></span>    | <span data-ttu-id="2a377-113">String</span><span class="sxs-lookup"><span data-stu-id="2a377-113">String</span></span> | <span data-ttu-id="2a377-114">Идентификатор преподавателя во внешней исходной системе.</span><span class="sxs-lookup"><span data-stu-id="2a377-114">Id of the Teacher in external source system.</span></span> |
| <span data-ttu-id="2a377-115">teacherNumber</span><span class="sxs-lookup"><span data-stu-id="2a377-115">teacherNumber</span></span> | <span data-ttu-id="2a377-116">String</span><span class="sxs-lookup"><span data-stu-id="2a377-116">String</span></span> | <span data-ttu-id="2a377-117">Номер преподавателя.</span><span class="sxs-lookup"><span data-stu-id="2a377-117">Teacher number.</span></span>                              |

## <a name="json-representation"></a><span data-ttu-id="2a377-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2a377-118">JSON representation</span></span>

<span data-ttu-id="2a377-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2a377-119">The following is a JSON representation of the resource.</span></span>

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


