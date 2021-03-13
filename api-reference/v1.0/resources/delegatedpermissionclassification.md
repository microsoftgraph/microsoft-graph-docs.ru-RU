---
title: тип ресурса delegatedPermissionClassification
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: ff9f4ca394e2065c69fd7cd08a19d60817fc4f99
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761760"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="7c62e-103">тип ресурса delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="7c62e-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="7c62e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c62e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7c62e-105">Используется для указания классификации делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="7c62e-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="7c62e-106">Делегированная классификация разрешений может использоваться в сочетании с настройками согласия пользователя для выбора разрешений, на которые разрешено согласие пользователя.</span><span class="sxs-lookup"><span data-stu-id="7c62e-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="7c62e-107">Подробнее о классификации разрешений см. в приложении Configure how [end-users consent to applications.](/azure/active-directory/manage-apps/configure-user-consent)</span><span class="sxs-lookup"><span data-stu-id="7c62e-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="7c62e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="7c62e-108">Properties</span></span>

| <span data-ttu-id="7c62e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="7c62e-109">Property</span></span> | <span data-ttu-id="7c62e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="7c62e-110">Type</span></span> | <span data-ttu-id="7c62e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="7c62e-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="7c62e-112">id</span><span class="sxs-lookup"><span data-stu-id="7c62e-112">id</span></span> | <span data-ttu-id="7c62e-113">String</span><span class="sxs-lookup"><span data-stu-id="7c62e-113">String</span></span> | <span data-ttu-id="7c62e-114">Уникальный идентификатор для ключа **делегированияPermissionClassification.**</span><span class="sxs-lookup"><span data-stu-id="7c62e-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="7c62e-115">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="7c62e-115">Not nullable.</span></span> <span data-ttu-id="7c62e-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="7c62e-116">Read-only.</span></span> |
| <span data-ttu-id="7c62e-117">classification</span><span class="sxs-lookup"><span data-stu-id="7c62e-117">classification</span></span> | <span data-ttu-id="7c62e-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="7c62e-118">permissionClassificationType</span></span> | <span data-ttu-id="7c62e-119">Задано значение классификации.</span><span class="sxs-lookup"><span data-stu-id="7c62e-119">The classification value being given.</span></span> <span data-ttu-id="7c62e-120">Возможное значение: `low` .</span><span class="sxs-lookup"><span data-stu-id="7c62e-120">Possible value: `low`.</span></span> <span data-ttu-id="7c62e-121">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7c62e-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="7c62e-122">permissionId</span><span class="sxs-lookup"><span data-stu-id="7c62e-122">permissionId</span></span> | <span data-ttu-id="7c62e-123">Guid</span><span class="sxs-lookup"><span data-stu-id="7c62e-123">Guid</span></span> | <span data-ttu-id="7c62e-124">Уникальный идентификатор **(id)** для делегированного разрешения, перечисленного в **коллекции oauth2PermissionScopes** [службыPrincipal.](servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="7c62e-124">The unique identifier (**id**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="7c62e-125">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="7c62e-125">Required on create.</span></span> <span data-ttu-id="7c62e-126">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7c62e-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="7c62e-127">permissionName</span><span class="sxs-lookup"><span data-stu-id="7c62e-127">permissionName</span></span> | <span data-ttu-id="7c62e-128">String</span><span class="sxs-lookup"><span data-stu-id="7c62e-128">String</span></span> | <span data-ttu-id="7c62e-129">Значение утверждения **(значение)** для делегированного разрешения, перечисленного в **коллекции oauth2PermissionScopes** [службыPrincipal.](servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="7c62e-129">The claim value (**value**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="7c62e-130">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="7c62e-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7c62e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7c62e-131">JSON representation</span></span>

<span data-ttu-id="7c62e-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="7c62e-132">The following is a JSON representation of the resource.</span></span>

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
