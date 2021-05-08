---
title: тип ресурса educationOrganization
description: Абстрактная сущность, используемая для моделирования общности между различными типами организаций в секторе образования.
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: b24313b6b6061449faea0ecb4880a421a2333099
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231866"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="df88a-103">тип ресурса educationOrganization</span><span class="sxs-lookup"><span data-stu-id="df88a-103">educationOrganization resource type</span></span>

<span data-ttu-id="df88a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df88a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df88a-105">Абстрактная сущность, используемая для моделирования общности между различными типами организаций в секторе образования.</span><span class="sxs-lookup"><span data-stu-id="df88a-105">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

<span data-ttu-id="df88a-106">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="df88a-106">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="properties"></a><span data-ttu-id="df88a-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="df88a-107">Properties</span></span>

| <span data-ttu-id="df88a-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="df88a-108">Property</span></span>             | <span data-ttu-id="df88a-109">Тип</span><span class="sxs-lookup"><span data-stu-id="df88a-109">Type</span></span>                    | <span data-ttu-id="df88a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="df88a-110">Description</span></span>                                                                            |
| :------------------- | :---------------------- | :------------------------------------------------------------------------------------- |
| <span data-ttu-id="df88a-111">description</span><span class="sxs-lookup"><span data-stu-id="df88a-111">description</span></span>          | <span data-ttu-id="df88a-112">Строка</span><span class="sxs-lookup"><span data-stu-id="df88a-112">String</span></span>                  | <span data-ttu-id="df88a-113">Описание организации.</span><span class="sxs-lookup"><span data-stu-id="df88a-113">Organization description.</span></span>                                                              |
| <span data-ttu-id="df88a-114">displayName</span><span class="sxs-lookup"><span data-stu-id="df88a-114">displayName</span></span>          | <span data-ttu-id="df88a-115">Строка</span><span class="sxs-lookup"><span data-stu-id="df88a-115">String</span></span>                  | <span data-ttu-id="df88a-116">Имя отображения организации.</span><span class="sxs-lookup"><span data-stu-id="df88a-116">Organization display name.</span></span>                                                             |
| <span data-ttu-id="df88a-117">externalSource</span><span class="sxs-lookup"><span data-stu-id="df88a-117">externalSource</span></span>       | <span data-ttu-id="df88a-118">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="df88a-118">educationExternalSource</span></span> | <span data-ttu-id="df88a-119">Источник, из которых была создана эта организация.</span><span class="sxs-lookup"><span data-stu-id="df88a-119">Source where this organization was created from.</span></span> <span data-ttu-id="df88a-120">Возможные значения: `sis`, `manual`.</span><span class="sxs-lookup"><span data-stu-id="df88a-120">Possible values are: `sis`, `manual`.</span></span> |
| <span data-ttu-id="df88a-121">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="df88a-121">externalSourceDetail</span></span> | <span data-ttu-id="df88a-122">Строка</span><span class="sxs-lookup"><span data-stu-id="df88a-122">String</span></span>                  | <span data-ttu-id="df88a-123">Имя внешнего источника, из которого были созданы эти ресурсы.</span><span class="sxs-lookup"><span data-stu-id="df88a-123">The name of the external source this resources was generated from.</span></span>                     |
| <span data-ttu-id="df88a-124">id</span><span class="sxs-lookup"><span data-stu-id="df88a-124">id</span></span>                   | <span data-ttu-id="df88a-125">Строка</span><span class="sxs-lookup"><span data-stu-id="df88a-125">String</span></span>                  | <span data-ttu-id="df88a-126">Идентификатор объекта.</span><span class="sxs-lookup"><span data-stu-id="df88a-126">Object identifier.</span></span> <span data-ttu-id="df88a-127">Унаследованный от [сущности](../resources/entity.md)</span><span class="sxs-lookup"><span data-stu-id="df88a-127">Inherited from [entity](../resources/entity.md)</span></span>                     |

## <a name="relationships"></a><span data-ttu-id="df88a-128">Связи</span><span class="sxs-lookup"><span data-stu-id="df88a-128">Relationships</span></span>

<span data-ttu-id="df88a-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="df88a-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="df88a-130">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="df88a-130">JSON representation</span></span>

<span data-ttu-id="df88a-131">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="df88a-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.educationOrganization",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationOrganization",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "externalSource": "String",
  "externalSourceDetail": "String"
}
```
