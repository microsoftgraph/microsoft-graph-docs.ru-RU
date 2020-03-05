---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления условиями использования функции Azure Active Directory в соответствии со сценарием.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9d45be38338554a1bf5181e4f7a3624b3d928127
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508389"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="84bd9-104">Тип ресурса договора</span><span class="sxs-lookup"><span data-stu-id="84bd9-104">agreement resource type</span></span>

<span data-ttu-id="84bd9-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="84bd9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="84bd9-106">Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="84bd9-106">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="84bd9-107">Вы можете использовать следующие методы для создания и управления [условиями использования функции Azure Active Directory](/azure/active-directory/active-directory-tou) в соответствии со сценарием.</span><span class="sxs-lookup"><span data-stu-id="84bd9-107">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="84bd9-108">Методы</span><span class="sxs-lookup"><span data-stu-id="84bd9-108">Methods</span></span>

| <span data-ttu-id="84bd9-109">Метод</span><span class="sxs-lookup"><span data-stu-id="84bd9-109">Method</span></span>       | <span data-ttu-id="84bd9-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="84bd9-110">Return Type</span></span> | <span data-ttu-id="84bd9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="84bd9-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="84bd9-112">Создание договоров</span><span class="sxs-lookup"><span data-stu-id="84bd9-112">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="84bd9-113">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="84bd9-113">agreement</span></span>](agreement.md) | <span data-ttu-id="84bd9-114">Создание нового соглашения путем публикации в коллекции договоров.</span><span class="sxs-lookup"><span data-stu-id="84bd9-114">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="84bd9-115">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="84bd9-115">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="84bd9-116">Коллекция [договоров](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="84bd9-116">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="84bd9-117">Получение коллекции объектов Agreement.</span><span class="sxs-lookup"><span data-stu-id="84bd9-117">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="84bd9-118">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="84bd9-118">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="84bd9-119">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="84bd9-119">agreement</span></span>](agreement.md) | <span data-ttu-id="84bd9-120">Чтение свойств и связей объекта Agreement.</span><span class="sxs-lookup"><span data-stu-id="84bd9-120">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="84bd9-121">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="84bd9-121">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="84bd9-122">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="84bd9-122">agreement</span></span>](agreement.md) | <span data-ttu-id="84bd9-123">Обновление объекта договора.</span><span class="sxs-lookup"><span data-stu-id="84bd9-123">Update an agreement object.</span></span> |
| [<span data-ttu-id="84bd9-124">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="84bd9-124">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="84bd9-125">Нет</span><span class="sxs-lookup"><span data-stu-id="84bd9-125">None</span></span> | <span data-ttu-id="84bd9-126">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="84bd9-126">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="84bd9-127">Свойства</span><span class="sxs-lookup"><span data-stu-id="84bd9-127">Properties</span></span>
| <span data-ttu-id="84bd9-128">Свойство</span><span class="sxs-lookup"><span data-stu-id="84bd9-128">Property</span></span>     | <span data-ttu-id="84bd9-129">Тип</span><span class="sxs-lookup"><span data-stu-id="84bd9-129">Type</span></span>        | <span data-ttu-id="84bd9-130">Описание</span><span class="sxs-lookup"><span data-stu-id="84bd9-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84bd9-131">displayName</span><span class="sxs-lookup"><span data-stu-id="84bd9-131">displayName</span></span>|<span data-ttu-id="84bd9-132">Строка</span><span class="sxs-lookup"><span data-stu-id="84bd9-132">String</span></span>|<span data-ttu-id="84bd9-133">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="84bd9-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="84bd9-134">id</span><span class="sxs-lookup"><span data-stu-id="84bd9-134">id</span></span>|<span data-ttu-id="84bd9-135">String</span><span class="sxs-lookup"><span data-stu-id="84bd9-135">String</span></span>| <span data-ttu-id="84bd9-136">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd9-136">Read-only.</span></span>|
|<span data-ttu-id="84bd9-137">исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="84bd9-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="84bd9-138">Логический</span><span class="sxs-lookup"><span data-stu-id="84bd9-138">Boolean</span></span>|<span data-ttu-id="84bd9-139">Указывает, должно ли пользователь развернуть и просмотреть Соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="84bd9-139">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84bd9-140">Связи</span><span class="sxs-lookup"><span data-stu-id="84bd9-140">Relationships</span></span>
| <span data-ttu-id="84bd9-141">Связь</span><span class="sxs-lookup"><span data-stu-id="84bd9-141">Relationship</span></span> | <span data-ttu-id="84bd9-142">Тип</span><span class="sxs-lookup"><span data-stu-id="84bd9-142">Type</span></span>        | <span data-ttu-id="84bd9-143">Описание</span><span class="sxs-lookup"><span data-stu-id="84bd9-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="84bd9-144">files</span><span class="sxs-lookup"><span data-stu-id="84bd9-144">files</span></span>|<span data-ttu-id="84bd9-145">Коллекция [агриментфиле](agreementfile.md)</span><span class="sxs-lookup"><span data-stu-id="84bd9-145">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="84bd9-146">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="84bd9-146">Read-only.</span></span> <span data-ttu-id="84bd9-147">Документы PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="84bd9-147">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="84bd9-148">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="84bd9-148">JSON representation</span></span>

<span data-ttu-id="84bd9-149">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="84bd9-149">The following is a JSON representation of the resource.</span></span>

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
