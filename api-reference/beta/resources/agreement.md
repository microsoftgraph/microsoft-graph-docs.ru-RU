---
title: Тип ресурса соглашения
description: Представляет клиента настраиваемый соглашение об условиях использования, который создается и управляется с помощью Azure Active Directory (Azure AD). Можно использовать следующие методы для создания и управления компонента Azure Active Directory условия использования согласно сценарию.
localization_priority: Normal
ms.openlocfilehash: b253877f1bf82e4fbc61cebaef3c1bce208d9cca
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513853"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="9177c-104">Тип ресурса соглашения</span><span class="sxs-lookup"><span data-stu-id="9177c-104">agreement resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9177c-105">Представляет клиента настраиваемый соглашение об условиях использования, который создается и управляется с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="9177c-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="9177c-106">Можно использовать следующие методы для создания и управления [Azure Active Directory условия использования компонента](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) согласно сценарию.</span><span class="sxs-lookup"><span data-stu-id="9177c-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="9177c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="9177c-107">Methods</span></span>

| <span data-ttu-id="9177c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="9177c-108">Method</span></span>       | <span data-ttu-id="9177c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="9177c-109">Return Type</span></span> | <span data-ttu-id="9177c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="9177c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="9177c-111">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="9177c-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="9177c-112">соглашения</span><span class="sxs-lookup"><span data-stu-id="9177c-112">agreement</span></span>](agreement.md) | <span data-ttu-id="9177c-113">Создайте новое соглашение с учета в коллекцию соглашения.</span><span class="sxs-lookup"><span data-stu-id="9177c-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="9177c-114">Соглашения по списку</span><span class="sxs-lookup"><span data-stu-id="9177c-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="9177c-115">[соглашение](agreement.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="9177c-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="9177c-116">Получение коллекции объектов соглашения.</span><span class="sxs-lookup"><span data-stu-id="9177c-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="9177c-117">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="9177c-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="9177c-118">соглашения</span><span class="sxs-lookup"><span data-stu-id="9177c-118">agreement</span></span>](agreement.md) | <span data-ttu-id="9177c-119">Чтение свойства и связи объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="9177c-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="9177c-120">Обновить соглашения</span><span class="sxs-lookup"><span data-stu-id="9177c-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="9177c-121">соглашения</span><span class="sxs-lookup"><span data-stu-id="9177c-121">agreement</span></span>](agreement.md) | <span data-ttu-id="9177c-122">Обновление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="9177c-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="9177c-123">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="9177c-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="9177c-124">Нет</span><span class="sxs-lookup"><span data-stu-id="9177c-124">None</span></span> | <span data-ttu-id="9177c-125">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="9177c-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="9177c-126">Свойства</span><span class="sxs-lookup"><span data-stu-id="9177c-126">Properties</span></span>
| <span data-ttu-id="9177c-127">Свойство</span><span class="sxs-lookup"><span data-stu-id="9177c-127">Property</span></span>     | <span data-ttu-id="9177c-128">Тип</span><span class="sxs-lookup"><span data-stu-id="9177c-128">Type</span></span>        | <span data-ttu-id="9177c-129">Описание</span><span class="sxs-lookup"><span data-stu-id="9177c-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9177c-130">displayName</span><span class="sxs-lookup"><span data-stu-id="9177c-130">displayName</span></span>|<span data-ttu-id="9177c-131">String</span><span class="sxs-lookup"><span data-stu-id="9177c-131">String</span></span>|<span data-ttu-id="9177c-132">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="9177c-132">Display name of the agreement.</span></span>|
|<span data-ttu-id="9177c-133">id</span><span class="sxs-lookup"><span data-stu-id="9177c-133">id</span></span>|<span data-ttu-id="9177c-134">String</span><span class="sxs-lookup"><span data-stu-id="9177c-134">String</span></span>| <span data-ttu-id="9177c-135">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9177c-135">Read-only.</span></span>|
|<span data-ttu-id="9177c-136">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="9177c-136">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="9177c-137">Логическое</span><span class="sxs-lookup"><span data-stu-id="9177c-137">Boolean</span></span>|<span data-ttu-id="9177c-138">Указывает, есть ли у пользователя можно развернуть и отобразить соглашения перед подтверждением.</span><span class="sxs-lookup"><span data-stu-id="9177c-138">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9177c-139">Отношения</span><span class="sxs-lookup"><span data-stu-id="9177c-139">Relationships</span></span>
| <span data-ttu-id="9177c-140">Связь</span><span class="sxs-lookup"><span data-stu-id="9177c-140">Relationship</span></span> | <span data-ttu-id="9177c-141">Тип</span><span class="sxs-lookup"><span data-stu-id="9177c-141">Type</span></span>        | <span data-ttu-id="9177c-142">Описание</span><span class="sxs-lookup"><span data-stu-id="9177c-142">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9177c-143">files</span><span class="sxs-lookup"><span data-stu-id="9177c-143">files</span></span>|<span data-ttu-id="9177c-144">[agreementFile](agreementfile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="9177c-144">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="9177c-145">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="9177c-145">Read-only.</span></span> <span data-ttu-id="9177c-146">PDF-файлы, связанные с этого соглашения.</span><span class="sxs-lookup"><span data-stu-id="9177c-146">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9177c-147">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9177c-147">JSON representation</span></span>

<span data-ttu-id="9177c-148">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9177c-148">The following is a JSON representation of the resource.</span></span>

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
