---
title: Тип ресурса Стсполици
description: Представляет абстрактный базовый тип для типов политики, которые управляют поведением платформы Microsoft Identity.
localization_priority: Normal
author: lujiangfeng666
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 911c790ab08487428ff04e93508f4f62ab657aa7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044209"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="e6b8b-103">Тип ресурса Стсполици</span><span class="sxs-lookup"><span data-stu-id="e6b8b-103">stsPolicy resource type</span></span>

<span data-ttu-id="e6b8b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6b8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6b8b-105">Представляет абстрактный базовый тип для типов политики, которые управляют поведением [платформы Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/) .</span><span class="sxs-lookup"><span data-stu-id="e6b8b-105">Represents an abstract base type for policy types that control [Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="e6b8b-106">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="e6b8b-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e6b8b-107">Методы</span><span class="sxs-lookup"><span data-stu-id="e6b8b-107">Methods</span></span>

<span data-ttu-id="e6b8b-108">Нет</span><span class="sxs-lookup"><span data-stu-id="e6b8b-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="e6b8b-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="e6b8b-109">Properties</span></span>

| <span data-ttu-id="e6b8b-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="e6b8b-110">Property</span></span>     | <span data-ttu-id="e6b8b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="e6b8b-111">Type</span></span>        | <span data-ttu-id="e6b8b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="e6b8b-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6b8b-113">id</span><span class="sxs-lookup"><span data-stu-id="e6b8b-113">id</span></span>|<span data-ttu-id="e6b8b-114">Строка</span><span class="sxs-lookup"><span data-stu-id="e6b8b-114">String</span></span>| <span data-ttu-id="e6b8b-115">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-115">Unique identifier for this policy.</span></span> <span data-ttu-id="e6b8b-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-116">Read-only.</span></span> <span data-ttu-id="e6b8b-117">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="e6b8b-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="e6b8b-118">description</span><span class="sxs-lookup"><span data-stu-id="e6b8b-118">description</span></span>|<span data-ttu-id="e6b8b-119">String</span><span class="sxs-lookup"><span data-stu-id="e6b8b-119">String</span></span>| <span data-ttu-id="e6b8b-120">Описание для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-120">Description for this policy.</span></span> <span data-ttu-id="e6b8b-121">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="e6b8b-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="e6b8b-122">displayName</span><span class="sxs-lookup"><span data-stu-id="e6b8b-122">displayName</span></span>|<span data-ttu-id="e6b8b-123">Строка</span><span class="sxs-lookup"><span data-stu-id="e6b8b-123">String</span></span>| <span data-ttu-id="e6b8b-124">Отображаемое имя для этой политики.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-124">Display name for this policy.</span></span> <span data-ttu-id="e6b8b-125">Наследуется от [основы](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="e6b8b-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="e6b8b-126">RDLC</span><span class="sxs-lookup"><span data-stu-id="e6b8b-126">definition</span></span>|<span data-ttu-id="e6b8b-127">Коллекция String</span><span class="sxs-lookup"><span data-stu-id="e6b8b-127">String collection</span></span>| <span data-ttu-id="e6b8b-128">Коллекция String, содержащая строку JSON, определяющую правила и параметры политики.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="e6b8b-129">Синтаксис определения отличается для каждого производного типа политики.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="e6b8b-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-130">Required.</span></span>|
|<span data-ttu-id="e6b8b-131">исорганизатиондефаулт</span><span class="sxs-lookup"><span data-stu-id="e6b8b-131">isOrganizationDefault</span></span>|<span data-ttu-id="e6b8b-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6b8b-132">Boolean</span></span>|<span data-ttu-id="e6b8b-133">Если задано значение true, активируется эта политика.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-133">If set to true, activates this policy.</span></span> <span data-ttu-id="e6b8b-134">Для одного и того же типа политики может быть задано несколько политик, но только одна из них может быть активирована в качестве организации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="e6b8b-135">Необязательное значение по умолчанию — false.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6b8b-136">Связи</span><span class="sxs-lookup"><span data-stu-id="e6b8b-136">Relationships</span></span>

<span data-ttu-id="e6b8b-137">Нет</span><span class="sxs-lookup"><span data-stu-id="e6b8b-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6b8b-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e6b8b-138">JSON representation</span></span>

<span data-ttu-id="e6b8b-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e6b8b-139">The following is a JSON representation of the resource.</span></span>

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


