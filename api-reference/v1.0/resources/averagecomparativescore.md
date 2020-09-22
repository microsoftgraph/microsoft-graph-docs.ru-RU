---
title: Тип ресурса Аверажекомпаративескоре
description: Содержит различные оценки на основе разных областей.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: bc104f3a9c19c38ef569d08d24da83d0e07d75f5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091903"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="c2e86-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="c2e86-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="c2e86-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2e86-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c2e86-105">Содержит различные оценки на основе различных областей (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="c2e86-105">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="c2e86-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="c2e86-106">Properties</span></span>

|<span data-ttu-id="c2e86-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="c2e86-107">Property</span></span> |<span data-ttu-id="c2e86-108">Тип</span><span class="sxs-lookup"><span data-stu-id="c2e86-108">Type</span></span> |<span data-ttu-id="c2e86-109">Описание</span><span class="sxs-lookup"><span data-stu-id="c2e86-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="c2e86-110">бы</span><span class="sxs-lookup"><span data-stu-id="c2e86-110">basis</span></span>|<span data-ttu-id="c2e86-111">Строка</span><span class="sxs-lookup"><span data-stu-id="c2e86-111">String</span></span>|<span data-ttu-id="c2e86-112">Тип области.</span><span class="sxs-lookup"><span data-stu-id="c2e86-112">Scope type.</span></span> <span data-ttu-id="c2e86-113">Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span><span class="sxs-lookup"><span data-stu-id="c2e86-113">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="c2e86-114">аверажескоре</span><span class="sxs-lookup"><span data-stu-id="c2e86-114">averageScore</span></span>|<span data-ttu-id="c2e86-115">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="c2e86-115">Double</span></span>|<span data-ttu-id="c2e86-116">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="c2e86-116">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c2e86-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c2e86-117">JSON representation</span></span>

<span data-ttu-id="c2e86-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c2e86-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.averageComparativeScore"
}-->

```json
{
  "basis": "String",
  "averageScore": "Double"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "averageComparativeScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

