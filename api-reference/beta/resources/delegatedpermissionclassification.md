---
title: Тип ресурса Делегатедпермиссионклассификатион
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f41ea807859b11982283b2a9743d6167e99dac66
ms.sourcegitcommit: 775b38baac6a4e7704d6144ef4589f2fc476bd61
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/13/2020
ms.locfileid: "48433704"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="522f6-103">Тип ресурса Делегатедпермиссионклассификатион</span><span class="sxs-lookup"><span data-stu-id="522f6-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="522f6-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="522f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="522f6-105">Используется для указания классификации делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="522f6-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="522f6-106">Делегированные классификации разрешений можно использовать в сочетании с параметрами согласия пользователя для выбора разрешений, на которые пользователю разрешено согласие.</span><span class="sxs-lookup"><span data-stu-id="522f6-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="522f6-107">Узнайте, [как конечные пользователи](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) могут узнать больше о классификациях разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="522f6-107">See [Configure how end-users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="522f6-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="522f6-108">Properties</span></span>

| <span data-ttu-id="522f6-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="522f6-109">Property</span></span> | <span data-ttu-id="522f6-110">Тип</span><span class="sxs-lookup"><span data-stu-id="522f6-110">Type</span></span> | <span data-ttu-id="522f6-111">Описание</span><span class="sxs-lookup"><span data-stu-id="522f6-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="522f6-112">id</span><span class="sxs-lookup"><span data-stu-id="522f6-112">id</span></span> | <span data-ttu-id="522f6-113">String</span><span class="sxs-lookup"><span data-stu-id="522f6-113">String</span></span> | <span data-ttu-id="522f6-114">Уникальный идентификатор для ключа **делегатедпермиссионклассификатион** .</span><span class="sxs-lookup"><span data-stu-id="522f6-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="522f6-115">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="522f6-115">Not nullable.</span></span> <span data-ttu-id="522f6-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="522f6-116">Read-only.</span></span> |
| <span data-ttu-id="522f6-117">classification</span><span class="sxs-lookup"><span data-stu-id="522f6-117">classification</span></span> | <span data-ttu-id="522f6-118">пермиссионклассификатионтипе</span><span class="sxs-lookup"><span data-stu-id="522f6-118">permissionClassificationType</span></span> | <span data-ttu-id="522f6-119">Заданное значение классификации.</span><span class="sxs-lookup"><span data-stu-id="522f6-119">The classification value being given.</span></span> <span data-ttu-id="522f6-120">Возможные значения: `low` .</span><span class="sxs-lookup"><span data-stu-id="522f6-120">Possible value: `low`.</span></span> <span data-ttu-id="522f6-121">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="522f6-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="522f6-122">пермиссионид</span><span class="sxs-lookup"><span data-stu-id="522f6-122">permissionId</span></span> | <span data-ttu-id="522f6-123">Guid</span><span class="sxs-lookup"><span data-stu-id="522f6-123">Guid</span></span> | <span data-ttu-id="522f6-124">Уникальный идентификатор (**ID**) для делегированного разрешения, указанного в коллекции **публишедпермиссионскопес** объекта [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="522f6-124">The unique identifier (**id**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="522f6-125">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="522f6-125">Required on create.</span></span> <span data-ttu-id="522f6-126">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="522f6-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="522f6-127">пермиссионнаме</span><span class="sxs-lookup"><span data-stu-id="522f6-127">permissionName</span></span> | <span data-ttu-id="522f6-128">String</span><span class="sxs-lookup"><span data-stu-id="522f6-128">String</span></span> | <span data-ttu-id="522f6-129">Значение утверждения (**value**) для делегированного разрешения, указанного в коллекции **публишедпермиссионскопес** объекта [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="522f6-129">The claim value (**value**) for the delegated permission listed in the **publishedPermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="522f6-130">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="522f6-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="522f6-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="522f6-131">JSON representation</span></span>

<span data-ttu-id="522f6-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="522f6-132">The following is a JSON representation of the resource.</span></span>

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
