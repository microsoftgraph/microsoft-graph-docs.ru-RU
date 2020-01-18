---
title: Тип ресурса Стсполици
description: Представляет абстрактный базовый тип для типов политики, которые управляют поведением платформы Microsoft Identity.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f351d994daba00f4465d934fe570b5db2e704ae9
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234448"
---
# <a name="policybase-resource-type"></a><span data-ttu-id="4f8b1-103">Тип ресурса основы</span><span class="sxs-lookup"><span data-stu-id="4f8b1-103">policyBase resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4f8b1-104">Представляет абстрактный базовый тип для типов политики, которые управляют поведением [платформы Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/) .</span><span class="sxs-lookup"><span data-stu-id="4f8b1-104">Represents an abstract base type for policy types that control [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="4f8b1-105">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="4f8b1-105">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="4f8b1-106">Методы</span><span class="sxs-lookup"><span data-stu-id="4f8b1-106">Methods</span></span>

<span data-ttu-id="4f8b1-107">Нет</span><span class="sxs-lookup"><span data-stu-id="4f8b1-107">None</span></span>

## <a name="properties"></a><span data-ttu-id="4f8b1-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="4f8b1-108">Properties</span></span>

| <span data-ttu-id="4f8b1-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="4f8b1-109">Property</span></span>     | <span data-ttu-id="4f8b1-110">Тип</span><span class="sxs-lookup"><span data-stu-id="4f8b1-110">Type</span></span>        | <span data-ttu-id="4f8b1-111">Описание</span><span class="sxs-lookup"><span data-stu-id="4f8b1-111">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4f8b1-112">id</span><span class="sxs-lookup"><span data-stu-id="4f8b1-112">id</span></span>|<span data-ttu-id="4f8b1-113">String</span><span class="sxs-lookup"><span data-stu-id="4f8b1-113">String</span></span>| <span data-ttu-id="4f8b1-114">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-114">Unique identifier for this policy.</span></span> <span data-ttu-id="4f8b1-115">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-115">Read-only.</span></span> <span data-ttu-id="4f8b1-116">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="4f8b1-116">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="4f8b1-117">description</span><span class="sxs-lookup"><span data-stu-id="4f8b1-117">description</span></span>|<span data-ttu-id="4f8b1-118">String</span><span class="sxs-lookup"><span data-stu-id="4f8b1-118">String</span></span>| <span data-ttu-id="4f8b1-119">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-119">Description for this policy.</span></span> <span data-ttu-id="4f8b1-120">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="4f8b1-120">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="4f8b1-121">displayName</span><span class="sxs-lookup"><span data-stu-id="4f8b1-121">displayName</span></span>|<span data-ttu-id="4f8b1-122">Строка</span><span class="sxs-lookup"><span data-stu-id="4f8b1-122">String</span></span>| <span data-ttu-id="4f8b1-123">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-123">Display name for this policy.</span></span> <span data-ttu-id="4f8b1-124">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="4f8b1-124">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="4f8b1-125">RDLC</span><span class="sxs-lookup"><span data-stu-id="4f8b1-125">definition</span></span>|<span data-ttu-id="4f8b1-126">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="4f8b1-126">String collection</span></span>| <span data-ttu-id="4f8b1-127">Коллекция String, содержащая строку JSON, определяющую правила и параметры политики.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-127">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="4f8b1-128">Синтаксис определения отличается для каждого производного типа политики.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-128">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="4f8b1-129">Обязательный элемент.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-129">Required.</span></span>|
|<span data-ttu-id="4f8b1-130">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="4f8b1-130">isOrganizationDefault</span></span>|<span data-ttu-id="4f8b1-131">Логический</span><span class="sxs-lookup"><span data-stu-id="4f8b1-131">Boolean</span></span>|<span data-ttu-id="4f8b1-132">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-132">If set to true, activates this policy.</span></span> <span data-ttu-id="4f8b1-133">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-133">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="4f8b1-134">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-134">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4f8b1-135">Связи</span><span class="sxs-lookup"><span data-stu-id="4f8b1-135">Relationships</span></span>

<span data-ttu-id="4f8b1-136">Нет</span><span class="sxs-lookup"><span data-stu-id="4f8b1-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4f8b1-137">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="4f8b1-137">JSON representation</span></span>

<span data-ttu-id="4f8b1-138">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="4f8b1-138">The following is a JSON representation of the resource.</span></span>

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