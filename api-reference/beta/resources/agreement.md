---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 6ac24e7a46441b59e621425517371db9227b4010
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218487"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="29f75-103">Тип ресурса договора</span><span class="sxs-lookup"><span data-stu-id="29f75-103">agreement resource type</span></span>

<span data-ttu-id="29f75-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29f75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29f75-105">Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="29f75-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="29f75-106">Вы можете использовать следующие методы для создания и управления [условиями использования функции Azure Active Directory](/azure/active-directory/active-directory-tou) в соответствии со сценарием.</span><span class="sxs-lookup"><span data-stu-id="29f75-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="29f75-107">Методы</span><span class="sxs-lookup"><span data-stu-id="29f75-107">Methods</span></span>

| <span data-ttu-id="29f75-108">Метод</span><span class="sxs-lookup"><span data-stu-id="29f75-108">Method</span></span>       | <span data-ttu-id="29f75-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="29f75-109">Return Type</span></span> | <span data-ttu-id="29f75-110">Описание</span><span class="sxs-lookup"><span data-stu-id="29f75-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="29f75-111">Создание договоров</span><span class="sxs-lookup"><span data-stu-id="29f75-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="29f75-112">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="29f75-112">agreement</span></span>](agreement.md) | <span data-ttu-id="29f75-113">Создание нового соглашения путем публикации в коллекции договоров.</span><span class="sxs-lookup"><span data-stu-id="29f75-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="29f75-114">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="29f75-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="29f75-115">Коллекция [договоров](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="29f75-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="29f75-116">Получение коллекции объектов Agreement.</span><span class="sxs-lookup"><span data-stu-id="29f75-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="29f75-117">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="29f75-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="29f75-118">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="29f75-118">agreement</span></span>](agreement.md) | <span data-ttu-id="29f75-119">Чтение свойств и связей объекта Agreement.</span><span class="sxs-lookup"><span data-stu-id="29f75-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="29f75-120">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="29f75-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="29f75-121">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="29f75-121">agreement</span></span>](agreement.md) | <span data-ttu-id="29f75-122">Обновление объекта договора.</span><span class="sxs-lookup"><span data-stu-id="29f75-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="29f75-123">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="29f75-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="29f75-124">Нет</span><span class="sxs-lookup"><span data-stu-id="29f75-124">None</span></span> | <span data-ttu-id="29f75-125">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="29f75-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="29f75-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="29f75-126">Properties</span></span>
| <span data-ttu-id="29f75-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="29f75-127">Property</span></span>     | <span data-ttu-id="29f75-128">Тип</span><span class="sxs-lookup"><span data-stu-id="29f75-128">Type</span></span>        | <span data-ttu-id="29f75-129">Описание</span><span class="sxs-lookup"><span data-stu-id="29f75-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29f75-130">displayName</span><span class="sxs-lookup"><span data-stu-id="29f75-130">displayName</span></span>|<span data-ttu-id="29f75-131">Строка</span><span class="sxs-lookup"><span data-stu-id="29f75-131">String</span></span>|<span data-ttu-id="29f75-132">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="29f75-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="29f75-133">id</span><span class="sxs-lookup"><span data-stu-id="29f75-133">id</span></span>|<span data-ttu-id="29f75-134">String</span><span class="sxs-lookup"><span data-stu-id="29f75-134">String</span></span>| <span data-ttu-id="29f75-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29f75-135">Read-only.</span></span>|
|<span data-ttu-id="29f75-136">исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="29f75-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="29f75-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="29f75-137">Boolean</span></span>|<span data-ttu-id="29f75-138">Указывает, должно ли пользователь развернуть и просмотреть Соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="29f75-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="29f75-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="29f75-139">Relationships</span></span>
| <span data-ttu-id="29f75-140">Связь</span><span class="sxs-lookup"><span data-stu-id="29f75-140">Relationship</span></span> | <span data-ttu-id="29f75-141">Тип</span><span class="sxs-lookup"><span data-stu-id="29f75-141">Type</span></span>        | <span data-ttu-id="29f75-142">Описание</span><span class="sxs-lookup"><span data-stu-id="29f75-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="29f75-143">files</span><span class="sxs-lookup"><span data-stu-id="29f75-143">files</span></span>|<span data-ttu-id="29f75-144">Коллекция [агриментфиле](agreementfile.md)</span><span class="sxs-lookup"><span data-stu-id="29f75-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="29f75-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="29f75-145">Read-only.</span></span> <span data-ttu-id="29f75-146">Документы PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="29f75-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="29f75-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="29f75-147">JSON representation</span></span>

<span data-ttu-id="29f75-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="29f75-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
