---
title: Тип ресурса Ентитлементманажементсеттингс
description: Представляет параметры на уровне клиента для управления обслуживанием Azure AD.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 84f34740bd5e16bb001cd3618edf4c4b669155f2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48052889"
---
# <a name="entitlementmanagementsettings-resource-type"></a><span data-ttu-id="38cbc-103">Тип ресурса Ентитлементманажементсеттингс</span><span class="sxs-lookup"><span data-stu-id="38cbc-103">entitlementManagementSettings resource type</span></span>

<span data-ttu-id="38cbc-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38cbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38cbc-105">Представляет параметры, управляющие поведением [управления обслуживанием Azure AD](entitlementmanagement-root.md).</span><span class="sxs-lookup"><span data-stu-id="38cbc-105">Represents settings that control the behavior of [Azure AD entitlement management](entitlementmanagement-root.md).</span></span>

## <a name="methods"></a><span data-ttu-id="38cbc-106">Методы</span><span class="sxs-lookup"><span data-stu-id="38cbc-106">Methods</span></span>

| <span data-ttu-id="38cbc-107">Метод</span><span class="sxs-lookup"><span data-stu-id="38cbc-107">Method</span></span>       | <span data-ttu-id="38cbc-108">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="38cbc-108">Return Type</span></span> | <span data-ttu-id="38cbc-109">Описание</span><span class="sxs-lookup"><span data-stu-id="38cbc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="38cbc-110">Получение</span><span class="sxs-lookup"><span data-stu-id="38cbc-110">Get</span></span>](../api/entitlementmanagementsettings-get.md) | [<span data-ttu-id="38cbc-111">ентитлементманажементсеттингс</span><span class="sxs-lookup"><span data-stu-id="38cbc-111">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="38cbc-112">Чтение свойств объекта **ентитлементманажементсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="38cbc-112">Read the properties of an **entitlementManagementSettings** object.</span></span> |
| [<span data-ttu-id="38cbc-113">Обновление</span><span class="sxs-lookup"><span data-stu-id="38cbc-113">Update</span></span>](../api/entitlementmanagementsettings-update.md) | [<span data-ttu-id="38cbc-114">ентитлементманажементсеттингс</span><span class="sxs-lookup"><span data-stu-id="38cbc-114">entitlementManagementSettings</span></span>](entitlementmanagementsettings.md) | <span data-ttu-id="38cbc-115">Обновление свойств объекта **ентитлементманажементсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="38cbc-115">Update the properties of an **entitlementManagementSettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="38cbc-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="38cbc-116">Properties</span></span>

| <span data-ttu-id="38cbc-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="38cbc-117">Property</span></span>     | <span data-ttu-id="38cbc-118">Тип</span><span class="sxs-lookup"><span data-stu-id="38cbc-118">Type</span></span>        | <span data-ttu-id="38cbc-119">Описание</span><span class="sxs-lookup"><span data-stu-id="38cbc-119">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="38cbc-120">екстерналусерлифециклеактион</span><span class="sxs-lookup"><span data-stu-id="38cbc-120">externalUserLifecycleAction</span></span>|<span data-ttu-id="38cbc-121">Строка</span><span class="sxs-lookup"><span data-stu-id="38cbc-121">String</span></span>|<span data-ttu-id="38cbc-122">Один из `None` , `BlockSignIn` или `BlockSignInAndDelete` .</span><span class="sxs-lookup"><span data-stu-id="38cbc-122">One of `None`, `BlockSignIn`, or `BlockSignInAndDelete`.</span></span> |
|<span data-ttu-id="38cbc-123">дайсунтилекстерналусерделетедафтерблоккед</span><span class="sxs-lookup"><span data-stu-id="38cbc-123">daysUntilExternalUserDeletedAfterBlocked</span></span>|<span data-ttu-id="38cbc-124">Int64</span><span class="sxs-lookup"><span data-stu-id="38cbc-124">Int64</span></span>|<span data-ttu-id="38cbc-125">Если `externalUserLifecycleAction` задано `BlockSignInAndDelete` , то количество дней после блокирования входа от внешнего пользователя до удаления учетной записи.</span><span class="sxs-lookup"><span data-stu-id="38cbc-125">If `externalUserLifecycleAction` is `BlockSignInAndDelete`, the number of days after an external user is blocked from sign in before their account is deleted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38cbc-126">Связи</span><span class="sxs-lookup"><span data-stu-id="38cbc-126">Relationships</span></span>

<span data-ttu-id="38cbc-127">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="38cbc-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="38cbc-128">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="38cbc-128">JSON representation</span></span>

<span data-ttu-id="38cbc-129">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38cbc-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.entitlementManagementSettings",
  "baseType": "",
  "keyProperty": ""
}-->

```json
{
  "externalUserLifecycleAction": "String",
  "daysUntilExternalUserDeletedAfterBlocked": 1
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "entitlementManagementSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


