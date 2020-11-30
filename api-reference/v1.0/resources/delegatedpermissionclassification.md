---
title: Тип ресурса Делегатедпермиссионклассификатион
description: Используется для указания классификации делегированного разрешения.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 7d5926bff0d7096080aa22fae49d0ed15c7d1fcd
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377419"
---
# <a name="delegatedpermissionclassification-resource-type"></a><span data-ttu-id="24da4-103">Тип ресурса Делегатедпермиссионклассификатион</span><span class="sxs-lookup"><span data-stu-id="24da4-103">delegatedPermissionClassification resource type</span></span>

<span data-ttu-id="24da4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24da4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24da4-105">Используется для указания классификации делегированного разрешения.</span><span class="sxs-lookup"><span data-stu-id="24da4-105">Used to specify the classification of a delegated permission.</span></span>

<span data-ttu-id="24da4-106">Делегированные классификации разрешений можно использовать в сочетании с параметрами согласия пользователя для выбора разрешений, на которые пользователю разрешено согласие.</span><span class="sxs-lookup"><span data-stu-id="24da4-106">Delegated permission classifications can be used in combination with user consent settings to choose which permissions a user is allowed to consent to.</span></span> <span data-ttu-id="24da4-107">Узнайте, [как конечные пользователи](/azure/active-directory/manage-apps/configure-user-consent) могут узнать больше о классификациях разрешений для приложений.</span><span class="sxs-lookup"><span data-stu-id="24da4-107">See [Configure how end-users consent to applications](/azure/active-directory/manage-apps/configure-user-consent) to learn more about permission classifications.</span></span>

## <a name="properties"></a><span data-ttu-id="24da4-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="24da4-108">Properties</span></span>

| <span data-ttu-id="24da4-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="24da4-109">Property</span></span> | <span data-ttu-id="24da4-110">Тип</span><span class="sxs-lookup"><span data-stu-id="24da4-110">Type</span></span> | <span data-ttu-id="24da4-111">Описание</span><span class="sxs-lookup"><span data-stu-id="24da4-111">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="24da4-112">id</span><span class="sxs-lookup"><span data-stu-id="24da4-112">id</span></span> | <span data-ttu-id="24da4-113">Строка</span><span class="sxs-lookup"><span data-stu-id="24da4-113">String</span></span> | <span data-ttu-id="24da4-114">Уникальный идентификатор для ключа **делегатедпермиссионклассификатион** .</span><span class="sxs-lookup"><span data-stu-id="24da4-114">A unique identifier for the **delegatedPermissionClassification** Key.</span></span> <span data-ttu-id="24da4-115">Значение null не допускается.</span><span class="sxs-lookup"><span data-stu-id="24da4-115">Not nullable.</span></span> <span data-ttu-id="24da4-116">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="24da4-116">Read-only.</span></span> |
| <span data-ttu-id="24da4-117">classification</span><span class="sxs-lookup"><span data-stu-id="24da4-117">classification</span></span> | <span data-ttu-id="24da4-118">пермиссионклассификатионтипе</span><span class="sxs-lookup"><span data-stu-id="24da4-118">permissionClassificationType</span></span> | <span data-ttu-id="24da4-119">Заданное значение классификации.</span><span class="sxs-lookup"><span data-stu-id="24da4-119">The classification value being given.</span></span> <span data-ttu-id="24da4-120">Возможные значения: `low` .</span><span class="sxs-lookup"><span data-stu-id="24da4-120">Possible value: `low`.</span></span> <span data-ttu-id="24da4-121">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="24da4-121">Does not support `$filter`.</span></span> |
| <span data-ttu-id="24da4-122">пермиссионид</span><span class="sxs-lookup"><span data-stu-id="24da4-122">permissionId</span></span> | <span data-ttu-id="24da4-123">Guid</span><span class="sxs-lookup"><span data-stu-id="24da4-123">Guid</span></span> | <span data-ttu-id="24da4-124">Уникальный идентификатор (**ID**) для делегированного разрешения, указанного в коллекции **oauth2PermissionScopes** объекта [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="24da4-124">The unique identifier (**id**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="24da4-125">Требуется при создании.</span><span class="sxs-lookup"><span data-stu-id="24da4-125">Required on create.</span></span> <span data-ttu-id="24da4-126">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="24da4-126">Does not support `$filter`.</span></span> |
| <span data-ttu-id="24da4-127">пермиссионнаме</span><span class="sxs-lookup"><span data-stu-id="24da4-127">permissionName</span></span> | <span data-ttu-id="24da4-128">Строка</span><span class="sxs-lookup"><span data-stu-id="24da4-128">String</span></span> | <span data-ttu-id="24da4-129">Значение утверждения (**value**) для делегированного разрешения, указанного в коллекции **oauth2PermissionScopes** объекта [servicePrincipal](servicePrincipal.md).</span><span class="sxs-lookup"><span data-stu-id="24da4-129">The claim value (**value**) for the delegated permission listed in the **oauth2PermissionScopes** collection of the [servicePrincipal](servicePrincipal.md).</span></span> <span data-ttu-id="24da4-130">Не поддерживает `$filter`.</span><span class="sxs-lookup"><span data-stu-id="24da4-130">Does not support `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24da4-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="24da4-131">JSON representation</span></span>

<span data-ttu-id="24da4-132">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="24da4-132">The following is a JSON representation of the resource.</span></span>

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
