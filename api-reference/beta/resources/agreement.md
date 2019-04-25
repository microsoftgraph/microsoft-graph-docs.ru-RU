---
title: Тип ресурса договора
description: Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD). Вы можете использовать следующие методы для создания и управления условиями использования функции Azure Active Directory в соответствии со сценарием.
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535750"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="1a6e6-104">Тип ресурса договора</span><span class="sxs-lookup"><span data-stu-id="1a6e6-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a6e6-105">Представляет настраиваемое соглашение об использовании клиента, которое создается и управляется с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1a6e6-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="1a6e6-106">Вы можете использовать следующие методы для создания и управления [условиями использования функции Azure Active Directory](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) в соответствии со сценарием.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="1a6e6-107">Методы</span><span class="sxs-lookup"><span data-stu-id="1a6e6-107">Methods</span></span>

| <span data-ttu-id="1a6e6-108">Метод</span><span class="sxs-lookup"><span data-stu-id="1a6e6-108">Method</span></span>       | <span data-ttu-id="1a6e6-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1a6e6-109">Return Type</span></span> | <span data-ttu-id="1a6e6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="1a6e6-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1a6e6-111">Создание договоров</span><span class="sxs-lookup"><span data-stu-id="1a6e6-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="1a6e6-112">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="1a6e6-112">agreement</span></span>](agreement.md) | <span data-ttu-id="1a6e6-113">Создание нового соглашения путем публикации в коллекции договоров.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="1a6e6-114">Список соглашений</span><span class="sxs-lookup"><span data-stu-id="1a6e6-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="1a6e6-115">Коллекция [договоров](agreement.md)</span><span class="sxs-lookup"><span data-stu-id="1a6e6-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="1a6e6-116">Получение коллекции объектов Agreement.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="1a6e6-117">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="1a6e6-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="1a6e6-118">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="1a6e6-118">agreement</span></span>](agreement.md) | <span data-ttu-id="1a6e6-119">Чтение свойств и связей объекта Agreement.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="1a6e6-120">Обновление соглашения</span><span class="sxs-lookup"><span data-stu-id="1a6e6-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="1a6e6-121">Корпоратив</span><span class="sxs-lookup"><span data-stu-id="1a6e6-121">agreement</span></span>](agreement.md) | <span data-ttu-id="1a6e6-122">Обновление объекта договора.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="1a6e6-123">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="1a6e6-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="1a6e6-124">Нет</span><span class="sxs-lookup"><span data-stu-id="1a6e6-124">None</span></span> | <span data-ttu-id="1a6e6-125">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="1a6e6-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="1a6e6-126">Properties</span></span>
| <span data-ttu-id="1a6e6-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="1a6e6-127">Property</span></span>     | <span data-ttu-id="1a6e6-128">Тип</span><span class="sxs-lookup"><span data-stu-id="1a6e6-128">Type</span></span>        | <span data-ttu-id="1a6e6-129">Описание</span><span class="sxs-lookup"><span data-stu-id="1a6e6-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1a6e6-130">displayName</span><span class="sxs-lookup"><span data-stu-id="1a6e6-130">displayName</span></span>|<span data-ttu-id="1a6e6-131">String</span><span class="sxs-lookup"><span data-stu-id="1a6e6-131">String</span></span>|<span data-ttu-id="1a6e6-132">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="1a6e6-133">id</span><span class="sxs-lookup"><span data-stu-id="1a6e6-133">id</span></span>|<span data-ttu-id="1a6e6-134">String</span><span class="sxs-lookup"><span data-stu-id="1a6e6-134">String</span></span>| <span data-ttu-id="1a6e6-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-135">Read-only.</span></span>|
|<span data-ttu-id="1a6e6-136">Исвиевингбефореакцептанцерекуиред</span><span class="sxs-lookup"><span data-stu-id="1a6e6-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="1a6e6-137">Логический</span><span class="sxs-lookup"><span data-stu-id="1a6e6-137">Boolean</span></span>|<span data-ttu-id="1a6e6-138">Указывает, должно ли пользователь развернуть и просмотреть Соглашение перед принятием.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a6e6-139">Связи</span><span class="sxs-lookup"><span data-stu-id="1a6e6-139">Relationships</span></span>
| <span data-ttu-id="1a6e6-140">Отношение</span><span class="sxs-lookup"><span data-stu-id="1a6e6-140">Relationship</span></span> | <span data-ttu-id="1a6e6-141">Тип</span><span class="sxs-lookup"><span data-stu-id="1a6e6-141">Type</span></span>        | <span data-ttu-id="1a6e6-142">Описание</span><span class="sxs-lookup"><span data-stu-id="1a6e6-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1a6e6-143">files</span><span class="sxs-lookup"><span data-stu-id="1a6e6-143">files</span></span>|<span data-ttu-id="1a6e6-144">Коллекция [агриментфиле](agreementfile.md)</span><span class="sxs-lookup"><span data-stu-id="1a6e6-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="1a6e6-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-145">Read-only.</span></span> <span data-ttu-id="1a6e6-146">Документы PDF, связанные с этим соглашением.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a6e6-147">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1a6e6-147">JSON representation</span></span>

<span data-ttu-id="1a6e6-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1a6e6-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
  "suppressions": [
    "Error: /api-reference/beta/resources/agreement.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
