---
title: Тип ресурса Делегатедпермиссионклассификатион
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f3d35c11ffe29feafed025b95c8f221e4f9ee4cb
ms.sourcegitcommit: 366178d3fc37439791061082da80a63fba2c27df
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/05/2020
ms.locfileid: "48921734"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="5032b-103">Тип ресурса Делегатедпермиссионклассификатион</span><span class="sxs-lookup"><span data-stu-id="5032b-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="5032b-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5032b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5032b-105">Используется для указания классификации делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="5032b-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="5032b-106">Делегированные классификации разрешений можно использовать в сочетании с параметрами согласия пользователя для выбора разрешений, на которые пользователю разрешено согласие.</span><span class="sxs-lookup"><span data-stu-id="5032b-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="5032b-107">Узнайте, [как конечные пользователи](/azure/active-directory/manage-apps/configure-user-consent) могут узнать больше о классификациях разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="5032b-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="5032b-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="5032b-108">Properties</span></span>

| <span data-ttu-id="5032b-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="5032b-109">Property</span></span> | <span data-ttu-id="5032b-110">Тип</span><span class="sxs-lookup"><span data-stu-id="5032b-110">Type</span></span> | <span data-ttu-id="5032b-111">Описание</span><span class="sxs-lookup"><span data-stu-id="5032b-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="5032b-112">id</span><span class="sxs-lookup"><span data-stu-id="5032b-112">id</span></span> | <span data-ttu-id="5032b-113">String</span><span class="sxs-lookup"><span data-stu-id="5032b-113">String</span></span> | <span data-ttu-id="5032b-114">Уникальный идентификатор для ключа **делегатедпермиссионклассификатион** .</span><span class="sxs-lookup"><span data-stu-id="5032b-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="5032b-115">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="5032b-115">Not nullable.</span></span> <span data-ttu-id="5032b-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="5032b-116">Read-only.</span></span> |
| <span data-ttu-id="5032b-117">classification</span><span class="sxs-lookup"><span data-stu-id="5032b-117">classification</span></span> | <span data-ttu-id="5032b-118">пермиссионклассификатионтипе</span><span class="sxs-lookup"><span data-stu-id="5032b-118">permissionClassificationType</span></span> | <span data-ttu-id="5032b-119">Заданное значение классификации.</span><span class="sxs-lookup"><span data-stu-id="5032b-119">The classification value being given.</span></span> <span data-ttu-id="5032b-120">Возможные значения: `low` .</span><span class="sxs-lookup"><span data-stu-id="5032b-120">Possible value: `low`.</span></span> <span data-ttu-id="5032b-121">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5032b-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="5032b-122">пермиссионид</span><span class="sxs-lookup"><span data-stu-id="5032b-122">permissionId</span></span> | <span data-ttu-id="5032b-123">Guid</span><span class="sxs-lookup"><span data-stu-id="5032b-123">Guid</span></span> | <span data-ttu-id="5032b-124">Уникальный идентификатор ( **ID** ) для делегированного разрешения, указанного в коллекции **публишедпермиссионскопес** объекта [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="5032b-124">The unique identifier ( **id** ) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="5032b-125">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="5032b-125">Required on create.</span></span> <span data-ttu-id="5032b-126">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5032b-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="5032b-127">пермиссионнаме</span><span class="sxs-lookup"><span data-stu-id="5032b-127">permissionName</span></span> | <span data-ttu-id="5032b-128">String</span><span class="sxs-lookup"><span data-stu-id="5032b-128">String</span></span> | <span data-ttu-id="5032b-129">Значение утверждения ( **value** ) для делегированного разрешения, указанного в коллекции **публишедпермиссионскопес** объекта [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="5032b-129">The claim value ( **value** ) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="5032b-130">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="5032b-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5032b-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="5032b-131">JSON representation</span></span>

<span data-ttu-id="5032b-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5032b-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.delegatedPermissionClassification"
}-->

```json
{
  "id": "string (identifier)",
  "classification": "low",
  "permissionId": "string",
  "permissionName": "string"
}
```
