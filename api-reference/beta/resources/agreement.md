---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления условиями использования функции Azure Active Directory в соответствии со сценарием.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 31c25211efbca8ae0f52a9348ad0531ea818397f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974539"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="0ac2a-104">Тип ресурса договора</span><span class="sxs-lookup"><span data-stu-id="0ac2a-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ac2a-105">Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="0ac2a-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="0ac2a-106">Вы можете использовать следующие методы для создания и управления [условиями использования функции Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) в соответствии со сценарием.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="0ac2a-107">Методы</span><span class="sxs-lookup"><span data-stu-id="0ac2a-107">Methods</span></span>

| <span data-ttu-id="0ac2a-108">Метод</span><span class="sxs-lookup"><span data-stu-id="0ac2a-108">Method</span></span>       | <span data-ttu-id="0ac2a-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="0ac2a-109">Return Type</span></span> | <span data-ttu-id="0ac2a-110">Описание</span><span class="sxs-lookup"><span data-stu-id="0ac2a-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="0ac2a-111">Создание договоров</span><span class="sxs-lookup"><span data-stu-id="0ac2a-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="0ac2a-112">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="0ac2a-112">agreement</span></span>](agreement.md) | <span data-ttu-id="0ac2a-113">Создание нового соглашения путем публикации в коллекции договоров.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="0ac2a-114">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="0ac2a-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="0ac2a-115">Коллекция [договоров](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="0ac2a-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="0ac2a-116">Получение коллекции объектов Agreement.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="0ac2a-117">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="0ac2a-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="0ac2a-118">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="0ac2a-118">agreement</span></span>](agreement.md) | <span data-ttu-id="0ac2a-119">Чтение свойств и связей объекта Agreement.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="0ac2a-120">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="0ac2a-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="0ac2a-121">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="0ac2a-121">agreement</span></span>](agreement.md) | <span data-ttu-id="0ac2a-122">Обновление объекта договора.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="0ac2a-123">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="0ac2a-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="0ac2a-124">Нет</span><span class="sxs-lookup"><span data-stu-id="0ac2a-124">None</span></span> | <span data-ttu-id="0ac2a-125">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="0ac2a-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="0ac2a-126">Properties</span></span>
| <span data-ttu-id="0ac2a-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="0ac2a-127">Property</span></span>     | <span data-ttu-id="0ac2a-128">Тип</span><span class="sxs-lookup"><span data-stu-id="0ac2a-128">Type</span></span>        | <span data-ttu-id="0ac2a-129">Описание</span><span class="sxs-lookup"><span data-stu-id="0ac2a-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ac2a-130">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac2a-130">displayName</span></span>|<span data-ttu-id="0ac2a-131">Строка</span><span class="sxs-lookup"><span data-stu-id="0ac2a-131">String</span></span>|<span data-ttu-id="0ac2a-132">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="0ac2a-133">id</span><span class="sxs-lookup"><span data-stu-id="0ac2a-133">id</span></span>|<span data-ttu-id="0ac2a-134">String</span><span class="sxs-lookup"><span data-stu-id="0ac2a-134">String</span></span>| <span data-ttu-id="0ac2a-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-135">Read-only.</span></span>|
|<span data-ttu-id="0ac2a-136">Исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="0ac2a-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="0ac2a-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac2a-137">Boolean</span></span>|<span data-ttu-id="0ac2a-138">Указывает, должно ли пользователь развернуть и просмотреть Соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0ac2a-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="0ac2a-139">Relationships</span></span>
| <span data-ttu-id="0ac2a-140">Отношение</span><span class="sxs-lookup"><span data-stu-id="0ac2a-140">Relationship</span></span> | <span data-ttu-id="0ac2a-141">Тип</span><span class="sxs-lookup"><span data-stu-id="0ac2a-141">Type</span></span>        | <span data-ttu-id="0ac2a-142">Описание</span><span class="sxs-lookup"><span data-stu-id="0ac2a-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0ac2a-143">files</span><span class="sxs-lookup"><span data-stu-id="0ac2a-143">files</span></span>|<span data-ttu-id="0ac2a-144">Коллекция [агриментфиле](agreementfile.md)</span><span class="sxs-lookup"><span data-stu-id="0ac2a-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="0ac2a-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-145">Read-only.</span></span> <span data-ttu-id="0ac2a-146">Документы PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0ac2a-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0ac2a-147">JSON representation</span></span>

<span data-ttu-id="0ac2a-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0ac2a-148">The following is a JSON representation of the resource.</span></span>

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
