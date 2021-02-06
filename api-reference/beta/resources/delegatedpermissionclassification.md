---
title: Тип ресурса delegatedPermissionClassification
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 4a567696d2adf0cd2a53cc2eb4d193ec1e1c2855
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133639"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="9e382-103">Тип ресурса delegatedPermissionClassification</span><span class="sxs-lookup"><span data-stu-id="9e382-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="9e382-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e382-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e382-105">Используется для указания классификации делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="9e382-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="9e382-106">Делегированную классификацию разрешений можно использовать в сочетании с настройками согласия пользователя, чтобы выбрать разрешения, на которые пользователь может дать согласие.</span><span class="sxs-lookup"><span data-stu-id="9e382-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="9e382-107">См. ["Настройка согласия конечных пользователей на использование](/azure/active-directory/manage-apps/configure-user-consent) приложений для получения дополнительных данных о классификациях разрешений".</span><span class="sxs-lookup"><span data-stu-id="9e382-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="9e382-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="9e382-108">Properties</span></span>

| <span data-ttu-id="9e382-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="9e382-109">Property</span></span> | <span data-ttu-id="9e382-110">Тип</span><span class="sxs-lookup"><span data-stu-id="9e382-110">Type</span></span> | <span data-ttu-id="9e382-111">Описание</span><span class="sxs-lookup"><span data-stu-id="9e382-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="9e382-112">id</span><span class="sxs-lookup"><span data-stu-id="9e382-112">id</span></span> | <span data-ttu-id="9e382-113">Строка</span><span class="sxs-lookup"><span data-stu-id="9e382-113">String</span></span> | <span data-ttu-id="9e382-114">Уникальный идентификатор ключа **delegatedPermissionClassification.**</span><span class="sxs-lookup"><span data-stu-id="9e382-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="9e382-115">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="9e382-115">Not nullable.</span></span> <span data-ttu-id="9e382-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9e382-116">Read-only.</span></span> |
| <span data-ttu-id="9e382-117">classification</span><span class="sxs-lookup"><span data-stu-id="9e382-117">classification</span></span> | <span data-ttu-id="9e382-118">permissionClassificationType</span><span class="sxs-lookup"><span data-stu-id="9e382-118">permissionClassificationType</span></span> | <span data-ttu-id="9e382-119">Заданный значение классификации.</span><span class="sxs-lookup"><span data-stu-id="9e382-119">The classification value being given.</span></span> <span data-ttu-id="9e382-120">Возможное значение: `low` .</span><span class="sxs-lookup"><span data-stu-id="9e382-120">Possible value: `low`.</span></span> <span data-ttu-id="9e382-121">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="9e382-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="9e382-122">permissionId</span><span class="sxs-lookup"><span data-stu-id="9e382-122">permissionId</span></span> | <span data-ttu-id="9e382-123">Guid</span><span class="sxs-lookup"><span data-stu-id="9e382-123">Guid</span></span> | <span data-ttu-id="9e382-124">Уникальный идентификатор **(идентификатор)** делегированного разрешения, перечисленного в коллекции **publishedPermissionScopes** [servicePrincipal.](servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="9e382-124">The unique identifier (**id**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="9e382-125">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="9e382-125">Required on create.</span></span> <span data-ttu-id="9e382-126">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="9e382-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="9e382-127">permissionName</span><span class="sxs-lookup"><span data-stu-id="9e382-127">permissionName</span></span> | <span data-ttu-id="9e382-128">Строка</span><span class="sxs-lookup"><span data-stu-id="9e382-128">String</span></span> | <span data-ttu-id="9e382-129">Значение утверждения **(значение)** для делегированного разрешения, перечисленного в коллекции **publishedPermissionScopes** [servicePrincipal.](servicePrincipal.md)</span><span class="sxs-lookup"><span data-stu-id="9e382-129">The claim value (**value**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="9e382-130">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="9e382-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9e382-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9e382-131">JSON representation</span></span>

<span data-ttu-id="9e382-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9e382-132">The following is a JSON representation of the resource.</span></span>

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

