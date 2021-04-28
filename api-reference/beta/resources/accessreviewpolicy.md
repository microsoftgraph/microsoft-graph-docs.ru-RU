---
title: тип ресурсов accessReviewPolicy
description: Политика обзоров доступа — это одинтон, который позволяет организациям управлять политикой проверки доступа на уровне каталогов.
author: kafen
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 02940987682d84aa3fc3dbb076c998abfe24bf8e
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/28/2021
ms.locfileid: "52068160"
---
# <a name="accessreviewpolicy-resource-type"></a><span data-ttu-id="08567-103">тип ресурсов accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="08567-103">accessReviewPolicy resource type</span></span>

<span data-ttu-id="08567-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08567-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08567-105">Политика проверки доступа — это одинтон, который позволяет администраторам управлять политиками проверки доступа на уровне каталогов.</span><span class="sxs-lookup"><span data-stu-id="08567-105">Access review policy is a singleton that enables administrators to manage directory-level access review policies.</span></span> <span data-ttu-id="08567-106">Например, администраторы могут использовать политику проверки доступа, чтобы включить и отключить возможность владельцев групп создавать отзывы о доступе в группах, которые им принадлежат.</span><span class="sxs-lookup"><span data-stu-id="08567-106">For example, administrators can use the access review policy to enable and disable the ability of group owners to create access reviews on groups that they own.</span></span>


<span data-ttu-id="08567-107">Наследует от [объекта](../resources/entity.md).</span><span class="sxs-lookup"><span data-stu-id="08567-107">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="08567-108">Методы</span><span class="sxs-lookup"><span data-stu-id="08567-108">Methods</span></span>
|<span data-ttu-id="08567-109">Метод</span><span class="sxs-lookup"><span data-stu-id="08567-109">Method</span></span>|<span data-ttu-id="08567-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="08567-110">Return type</span></span>|<span data-ttu-id="08567-111">Описание</span><span class="sxs-lookup"><span data-stu-id="08567-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="08567-112">Получить accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="08567-112">Get accessReviewPolicy</span></span>](../api/accessreviewpolicy-get.md)|[<span data-ttu-id="08567-113">accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="08567-113">accessReviewPolicy</span></span>](../resources/accessreviewpolicy.md)|<span data-ttu-id="08567-114">Ознакомьтесь с свойствами и отношениями [объекта accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="08567-114">Read the properties and relationships of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>|
|[<span data-ttu-id="08567-115">Обновление accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="08567-115">Update accessReviewPolicy</span></span>](../api/accessreviewpolicy-update.md)|[<span data-ttu-id="08567-116">accessReviewPolicy</span><span class="sxs-lookup"><span data-stu-id="08567-116">accessReviewPolicy</span></span>](../resources/accessreviewpolicy.md)|<span data-ttu-id="08567-117">Обновление свойств объекта [accessReviewPolicy.](../resources/accessreviewpolicy.md)</span><span class="sxs-lookup"><span data-stu-id="08567-117">Update the properties of an [accessReviewPolicy](../resources/accessreviewpolicy.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="08567-118">Свойства</span><span class="sxs-lookup"><span data-stu-id="08567-118">Properties</span></span>
|<span data-ttu-id="08567-119">Свойство</span><span class="sxs-lookup"><span data-stu-id="08567-119">Property</span></span>|<span data-ttu-id="08567-120">Тип</span><span class="sxs-lookup"><span data-stu-id="08567-120">Type</span></span>|<span data-ttu-id="08567-121">Описание</span><span class="sxs-lookup"><span data-stu-id="08567-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08567-122">description</span><span class="sxs-lookup"><span data-stu-id="08567-122">description</span></span>|<span data-ttu-id="08567-123">String</span><span class="sxs-lookup"><span data-stu-id="08567-123">String</span></span>|<span data-ttu-id="08567-124">Описание этой политики.</span><span class="sxs-lookup"><span data-stu-id="08567-124">Description for this policy.</span></span> <span data-ttu-id="08567-125">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08567-125">Read-only.</span></span>|
|<span data-ttu-id="08567-126">displayName</span><span class="sxs-lookup"><span data-stu-id="08567-126">displayName</span></span>|<span data-ttu-id="08567-127">String</span><span class="sxs-lookup"><span data-stu-id="08567-127">String</span></span>|<span data-ttu-id="08567-128">Отображение имени для этой политики.</span><span class="sxs-lookup"><span data-stu-id="08567-128">Display name for this policy.</span></span> <span data-ttu-id="08567-129">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="08567-129">Read-only.</span></span>|
|<span data-ttu-id="08567-130">isGroupOwnerManagementEnabled</span><span class="sxs-lookup"><span data-stu-id="08567-130">isGroupOwnerManagementEnabled</span></span>|<span data-ttu-id="08567-131">Логический</span><span class="sxs-lookup"><span data-stu-id="08567-131">Boolean</span></span>|<span data-ttu-id="08567-132">Если `true` владельцы групп могут создавать и управлять отзывами доступа в группах, которые им принадлежат.</span><span class="sxs-lookup"><span data-stu-id="08567-132">If `true`, group owners can create and manage access reviews on groups they own.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08567-133">Связи</span><span class="sxs-lookup"><span data-stu-id="08567-133">Relationships</span></span>
<span data-ttu-id="08567-134">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="08567-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="08567-135">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="08567-135">JSON representation</span></span>
<span data-ttu-id="08567-136">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="08567-136">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessReviewPolicy",
  "displayName": "Access Review Policy",
  "description": "Policy contains directory-level access review settings.",
  "isGroupOwnerManagementEnabled": false
}
```
