---
title: Тип ресурса Стсполици
description: Представляет абстрактный базовый тип для типов политики, которые управляют поведением платформы Microsoft Identity.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 078284cb4134b0b4fa2f86eb9a09f61ab6655351
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405283"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="3a4ba-103">Тип ресурса Стсполици</span><span class="sxs-lookup"><span data-stu-id="3a4ba-103">stsPolicy resource type</span></span>

<span data-ttu-id="3a4ba-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a4ba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3a4ba-105">Представляет абстрактный базовый тип для типов политики, которые управляют поведением [платформы Microsoft Identity](/azure/active-directory/develop/) .</span><span class="sxs-lookup"><span data-stu-id="3a4ba-105">Represents an abstract base type for policy types that control [Microsoft identity platform](/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="3a4ba-106">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="3a4ba-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="3a4ba-107">Методы</span><span class="sxs-lookup"><span data-stu-id="3a4ba-107">Methods</span></span>

<span data-ttu-id="3a4ba-108">Нет</span><span class="sxs-lookup"><span data-stu-id="3a4ba-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="3a4ba-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="3a4ba-109">Properties</span></span>

| <span data-ttu-id="3a4ba-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="3a4ba-110">Property</span></span>     | <span data-ttu-id="3a4ba-111">Тип</span><span class="sxs-lookup"><span data-stu-id="3a4ba-111">Type</span></span>        | <span data-ttu-id="3a4ba-112">Описание</span><span class="sxs-lookup"><span data-stu-id="3a4ba-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3a4ba-113">id</span><span class="sxs-lookup"><span data-stu-id="3a4ba-113">id</span></span>|<span data-ttu-id="3a4ba-114">String</span><span class="sxs-lookup"><span data-stu-id="3a4ba-114">String</span></span>| <span data-ttu-id="3a4ba-115">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-115">Unique identifier for this policy.</span></span> <span data-ttu-id="3a4ba-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-116">Read-only.</span></span> <span data-ttu-id="3a4ba-117">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="3a4ba-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="3a4ba-118">description</span><span class="sxs-lookup"><span data-stu-id="3a4ba-118">description</span></span>|<span data-ttu-id="3a4ba-119">String</span><span class="sxs-lookup"><span data-stu-id="3a4ba-119">String</span></span>| <span data-ttu-id="3a4ba-120">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-120">Description for this policy.</span></span> <span data-ttu-id="3a4ba-121">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="3a4ba-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="3a4ba-122">displayName</span><span class="sxs-lookup"><span data-stu-id="3a4ba-122">displayName</span></span>|<span data-ttu-id="3a4ba-123">String</span><span class="sxs-lookup"><span data-stu-id="3a4ba-123">String</span></span>| <span data-ttu-id="3a4ba-124">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-124">Display name for this policy.</span></span> <span data-ttu-id="3a4ba-125">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="3a4ba-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="3a4ba-126">RDLC</span><span class="sxs-lookup"><span data-stu-id="3a4ba-126">definition</span></span>|<span data-ttu-id="3a4ba-127">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="3a4ba-127">String collection</span></span>| <span data-ttu-id="3a4ba-128">Коллекция String, содержащая строку JSON, определяющую правила и параметры политики.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="3a4ba-129">Синтаксис определения отличается для каждого производного типа политики.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="3a4ba-130">Обязательно.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-130">Required.</span></span>|
|<span data-ttu-id="3a4ba-131">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="3a4ba-131">isOrganizationDefault</span></span>|<span data-ttu-id="3a4ba-132">Логический</span><span class="sxs-lookup"><span data-stu-id="3a4ba-132">Boolean</span></span>|<span data-ttu-id="3a4ba-133">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-133">If set to true, activates this policy.</span></span> <span data-ttu-id="3a4ba-134">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="3a4ba-135">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3a4ba-136">Связи</span><span class="sxs-lookup"><span data-stu-id="3a4ba-136">Relationships</span></span>

<span data-ttu-id="3a4ba-137">Нет</span><span class="sxs-lookup"><span data-stu-id="3a4ba-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a4ba-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3a4ba-138">JSON representation</span></span>

<span data-ttu-id="3a4ba-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3a4ba-139">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stsPolicy",
  "baseType": "microsoft.graph.policyBase",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "definition": ["String"],
  "isOrganizationDefault": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stsPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->