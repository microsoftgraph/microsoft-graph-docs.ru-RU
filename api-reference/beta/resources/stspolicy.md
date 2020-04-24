---
title: Тип ресурса Стсполици
description: Представляет абстрактный базовый тип для типов политики, которые управляют поведением платформы Microsoft Identity.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 33582c39d8abe03e04a064935a5f3d0d70a330f7
ms.sourcegitcommit: 195fa0d441a49662e144323d37518dbba0c76fc7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2020
ms.locfileid: "43805681"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="a7267-103">Тип ресурса Стсполици</span><span class="sxs-lookup"><span data-stu-id="a7267-103">stsPolicy resource type</span></span>

<span data-ttu-id="a7267-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7267-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7267-105">Представляет абстрактный базовый тип для типов политики, которые управляют поведением [платформы Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/) .</span><span class="sxs-lookup"><span data-stu-id="a7267-105">Represents an abstract base type for policy types that control [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="a7267-106">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="a7267-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a7267-107">Methods</span><span class="sxs-lookup"><span data-stu-id="a7267-107">Methods</span></span>

<span data-ttu-id="a7267-108">Нет</span><span class="sxs-lookup"><span data-stu-id="a7267-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="a7267-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="a7267-109">Properties</span></span>

| <span data-ttu-id="a7267-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="a7267-110">Property</span></span>     | <span data-ttu-id="a7267-111">Тип</span><span class="sxs-lookup"><span data-stu-id="a7267-111">Type</span></span>        | <span data-ttu-id="a7267-112">Описание</span><span class="sxs-lookup"><span data-stu-id="a7267-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a7267-113">id</span><span class="sxs-lookup"><span data-stu-id="a7267-113">id</span></span>|<span data-ttu-id="a7267-114">String</span><span class="sxs-lookup"><span data-stu-id="a7267-114">String</span></span>| <span data-ttu-id="a7267-115">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a7267-115">Unique identifier for this policy.</span></span> <span data-ttu-id="a7267-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="a7267-116">Read-only.</span></span> <span data-ttu-id="a7267-117">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="a7267-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="a7267-118">description</span><span class="sxs-lookup"><span data-stu-id="a7267-118">description</span></span>|<span data-ttu-id="a7267-119">String</span><span class="sxs-lookup"><span data-stu-id="a7267-119">String</span></span>| <span data-ttu-id="a7267-120">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a7267-120">Description for this policy.</span></span> <span data-ttu-id="a7267-121">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="a7267-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="a7267-122">displayName</span><span class="sxs-lookup"><span data-stu-id="a7267-122">displayName</span></span>|<span data-ttu-id="a7267-123">Строка</span><span class="sxs-lookup"><span data-stu-id="a7267-123">String</span></span>| <span data-ttu-id="a7267-124">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="a7267-124">Display name for this policy.</span></span> <span data-ttu-id="a7267-125">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="a7267-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="a7267-126">RDLC</span><span class="sxs-lookup"><span data-stu-id="a7267-126">definition</span></span>|<span data-ttu-id="a7267-127">Коллекция объектов string</span><span class="sxs-lookup"><span data-stu-id="a7267-127">String collection</span></span>| <span data-ttu-id="a7267-128">Коллекция String, содержащая строку JSON, определяющую правила и параметры политики.</span><span class="sxs-lookup"><span data-stu-id="a7267-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="a7267-129">Синтаксис определения отличается для каждого производного типа политики.</span><span class="sxs-lookup"><span data-stu-id="a7267-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="a7267-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="a7267-130">Required.</span></span>|
|<span data-ttu-id="a7267-131">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="a7267-131">isOrganizationDefault</span></span>|<span data-ttu-id="a7267-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7267-132">Boolean</span></span>|<span data-ttu-id="a7267-133">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="a7267-133">If set to true, activates this policy.</span></span> <span data-ttu-id="a7267-134">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="a7267-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="a7267-135">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="a7267-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a7267-136">Связи</span><span class="sxs-lookup"><span data-stu-id="a7267-136">Relationships</span></span>

<span data-ttu-id="a7267-137">Нет</span><span class="sxs-lookup"><span data-stu-id="a7267-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7267-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a7267-138">JSON representation</span></span>

<span data-ttu-id="a7267-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a7267-139">The following is a JSON representation of the resource.</span></span>

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
