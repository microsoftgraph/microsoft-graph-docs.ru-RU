---
title: Тип ресурса Аверажекомпаративескоре
description: Содержит различные оценки на основе разных областей.
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1ed82e040121f49bdef29009f6ac387ed4c79cbc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532030"
---
#  <a name="averagecomparativescore-resource-type"></a><span data-ttu-id="2f37e-103">Тип ресурса Аверажекомпаративескоре</span><span class="sxs-lookup"><span data-stu-id="2f37e-103">averageComparativeScore resource type</span></span>

<span data-ttu-id="2f37e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f37e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2f37e-105">Содержит различные оценки на основе различных областей (например, усреднение по отраслевым вертикали, среднее значение по размеру компании и т. д.) и категории элементов управления (идентификация, данные, устройство, приложения, инфраструктура).</span><span class="sxs-lookup"><span data-stu-id="2f37e-105">Contains various different scores based on different scopes (for example, average by industry vertical, average by company seat size, and so on) and control category (Identity, Data, Device, Apps, Infrastructure).</span></span>

## <a name="properties"></a><span data-ttu-id="2f37e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="2f37e-106">Properties</span></span>

|<span data-ttu-id="2f37e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="2f37e-107">Property</span></span> |<span data-ttu-id="2f37e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="2f37e-108">Type</span></span> |<span data-ttu-id="2f37e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="2f37e-109">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="2f37e-110">бы</span><span class="sxs-lookup"><span data-stu-id="2f37e-110">basis</span></span>|<span data-ttu-id="2f37e-111">String</span><span class="sxs-lookup"><span data-stu-id="2f37e-111">String</span></span>|<span data-ttu-id="2f37e-112">Тип области.</span><span class="sxs-lookup"><span data-stu-id="2f37e-112">Scope type.</span></span> <span data-ttu-id="2f37e-113">Допустимые значения: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span><span class="sxs-lookup"><span data-stu-id="2f37e-113">The possible values are: `AllTenants`, `TotalSeats`, `IndustryTypes`.</span></span>|
|<span data-ttu-id="2f37e-114">аверажескоре</span><span class="sxs-lookup"><span data-stu-id="2f37e-114">averageScore</span></span>|<span data-ttu-id="2f37e-115">Двойное с плавающей точкой</span><span class="sxs-lookup"><span data-stu-id="2f37e-115">Double</span></span>|<span data-ttu-id="2f37e-116">Средняя оценка в указанном базисе.</span><span class="sxs-lookup"><span data-stu-id="2f37e-116">Average score within specified basis.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f37e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2f37e-117">JSON representation</span></span>

<span data-ttu-id="2f37e-118">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2f37e-118">The following is a JSON representation of the resource.</span></span>

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
