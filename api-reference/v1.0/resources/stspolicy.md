---
title: тип ресурсов stsPolicy
description: Представляет абстрактный базовый тип для типов политик, которые контролируют поведение платформы удостоверений Майкрософт.
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: ba7afc9d338a0fd34b5548ca2ade69eebfecf29c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760892"
---
# <a name="stspolicy-resource-type"></a><span data-ttu-id="041f7-103">тип ресурсов stsPolicy</span><span class="sxs-lookup"><span data-stu-id="041f7-103">stsPolicy resource type</span></span>

<span data-ttu-id="041f7-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="041f7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="041f7-105">Представляет абстрактный базовый тип для типов политик, которые контролируют [поведение платформы удостоверений](/azure/active-directory/develop/) Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="041f7-105">Represents an abstract base type for policy types that control [Microsoft identity platform](/azure/active-directory/develop/) behavior.</span></span>

<span data-ttu-id="041f7-106">Наследует [от policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="041f7-106">Inherits from [policyBase](policyBase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="041f7-107">Методы</span><span class="sxs-lookup"><span data-stu-id="041f7-107">Methods</span></span>

<span data-ttu-id="041f7-108">Нет</span><span class="sxs-lookup"><span data-stu-id="041f7-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="041f7-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="041f7-109">Properties</span></span>

| <span data-ttu-id="041f7-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="041f7-110">Property</span></span>     | <span data-ttu-id="041f7-111">Тип</span><span class="sxs-lookup"><span data-stu-id="041f7-111">Type</span></span>        | <span data-ttu-id="041f7-112">Описание</span><span class="sxs-lookup"><span data-stu-id="041f7-112">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="041f7-113">id</span><span class="sxs-lookup"><span data-stu-id="041f7-113">id</span></span>|<span data-ttu-id="041f7-114">String</span><span class="sxs-lookup"><span data-stu-id="041f7-114">String</span></span>| <span data-ttu-id="041f7-115">Уникальный идентификатор для этой политики.</span><span class="sxs-lookup"><span data-stu-id="041f7-115">Unique identifier for this policy.</span></span> <span data-ttu-id="041f7-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="041f7-116">Read-only.</span></span> <span data-ttu-id="041f7-117">Унаследованный от [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="041f7-117">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="041f7-118">description</span><span class="sxs-lookup"><span data-stu-id="041f7-118">description</span></span>|<span data-ttu-id="041f7-119">String</span><span class="sxs-lookup"><span data-stu-id="041f7-119">String</span></span>| <span data-ttu-id="041f7-120">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="041f7-120">Description for this policy.</span></span> <span data-ttu-id="041f7-121">Унаследованный от [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="041f7-121">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="041f7-122">displayName</span><span class="sxs-lookup"><span data-stu-id="041f7-122">displayName</span></span>|<span data-ttu-id="041f7-123">String</span><span class="sxs-lookup"><span data-stu-id="041f7-123">String</span></span>| <span data-ttu-id="041f7-124">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="041f7-124">Display name for this policy.</span></span> <span data-ttu-id="041f7-125">Унаследованный от [policyBase](policyBase.md).</span><span class="sxs-lookup"><span data-stu-id="041f7-125">Inherited from [policyBase](policyBase.md).</span></span>|
|<span data-ttu-id="041f7-126">определение</span><span class="sxs-lookup"><span data-stu-id="041f7-126">definition</span></span>|<span data-ttu-id="041f7-127">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="041f7-127">String collection</span></span>| <span data-ttu-id="041f7-128">Коллекция строк, содержащая строку JSON, определяемую правилами и настройками политики.</span><span class="sxs-lookup"><span data-stu-id="041f7-128">A string collection containing a JSON string that defines the rules and settings for a policy.</span></span> <span data-ttu-id="041f7-129">Синтаксис определения отличается для каждого типа политики.</span><span class="sxs-lookup"><span data-stu-id="041f7-129">The syntax for the definition differs for each derived policy type.</span></span> <span data-ttu-id="041f7-130">Обязательный.</span><span class="sxs-lookup"><span data-stu-id="041f7-130">Required.</span></span>|
|<span data-ttu-id="041f7-131">isOrganizationDefault</span><span class="sxs-lookup"><span data-stu-id="041f7-131">isOrganizationDefault</span></span>|<span data-ttu-id="041f7-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="041f7-132">Boolean</span></span>|<span data-ttu-id="041f7-133">Если заданной для true, активирует эту политику.</span><span class="sxs-lookup"><span data-stu-id="041f7-133">If set to true, activates this policy.</span></span> <span data-ttu-id="041f7-134">Для одного типа политики может быть много политик, но только одна может быть активирована по умолчанию организации.</span><span class="sxs-lookup"><span data-stu-id="041f7-134">There can be many policies for the same policy type, but only one can be activated as the organization default.</span></span> <span data-ttu-id="041f7-135">Необязательный, значение по умолчанию является ложным.</span><span class="sxs-lookup"><span data-stu-id="041f7-135">Optional, default value is false.</span></span>|

## <a name="relationships"></a><span data-ttu-id="041f7-136">Связи</span><span class="sxs-lookup"><span data-stu-id="041f7-136">Relationships</span></span>

<span data-ttu-id="041f7-137">Нет</span><span class="sxs-lookup"><span data-stu-id="041f7-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="041f7-138">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="041f7-138">JSON representation</span></span>

<span data-ttu-id="041f7-139">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="041f7-139">The following is a JSON representation of the resource.</span></span>

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