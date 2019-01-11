---
title: Тип ресурса соглашения
description: Представляет клиента настраиваемый соглашение об условиях использования, который создается и управляется с помощью Azure Active Directory (Azure AD). Можно использовать следующие методы для создания и управления компонента Azure Active Directory условия использования согласно сценарию.
localization_priority: Normal
ms.openlocfilehash: 8c082ed6229b44cc3a3d4cba6dd8645feee5d07c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845348"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="1b4b5-104">Тип ресурса соглашения</span><span class="sxs-lookup"><span data-stu-id="1b4b5-104">agreement resource type</span></span>

> <span data-ttu-id="1b4b5-105">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b4b5-106">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1b4b5-107">Представляет клиента настраиваемый соглашение об условиях использования, который создается и управляется с помощью Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="1b4b5-107">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="1b4b5-108">Можно использовать следующие методы для создания и управления [Azure Active Directory условия использования компонента](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) согласно сценарию.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-108">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="1b4b5-109">Методы</span><span class="sxs-lookup"><span data-stu-id="1b4b5-109">Methods</span></span>

| <span data-ttu-id="1b4b5-110">Метод</span><span class="sxs-lookup"><span data-stu-id="1b4b5-110">Method</span></span>       | <span data-ttu-id="1b4b5-111">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="1b4b5-111">Return Type</span></span> | <span data-ttu-id="1b4b5-112">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4b5-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1b4b5-113">Создание соглашения</span><span class="sxs-lookup"><span data-stu-id="1b4b5-113">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="1b4b5-114">соглашения</span><span class="sxs-lookup"><span data-stu-id="1b4b5-114">agreement</span></span>](agreement.md) | <span data-ttu-id="1b4b5-115">Создайте новое соглашение с учета в коллекцию соглашения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-115">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="1b4b5-116">Соглашения по списку</span><span class="sxs-lookup"><span data-stu-id="1b4b5-116">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="1b4b5-117">[соглашение](agreement.md) семейства сайтов</span><span class="sxs-lookup"><span data-stu-id="1b4b5-117">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="1b4b5-118">Получение коллекции объектов соглашения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-118">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="1b4b5-119">Получение соглашения</span><span class="sxs-lookup"><span data-stu-id="1b4b5-119">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="1b4b5-120">соглашения</span><span class="sxs-lookup"><span data-stu-id="1b4b5-120">agreement</span></span>](agreement.md) | <span data-ttu-id="1b4b5-121">Чтение свойства и связи объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-121">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="1b4b5-122">Обновить соглашения</span><span class="sxs-lookup"><span data-stu-id="1b4b5-122">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="1b4b5-123">соглашения</span><span class="sxs-lookup"><span data-stu-id="1b4b5-123">agreement</span></span>](agreement.md) | <span data-ttu-id="1b4b5-124">Обновление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-124">Update an agreement object.</span></span> |
| [<span data-ttu-id="1b4b5-125">Удаление соглашения</span><span class="sxs-lookup"><span data-stu-id="1b4b5-125">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="1b4b5-126">Нет</span><span class="sxs-lookup"><span data-stu-id="1b4b5-126">None</span></span> | <span data-ttu-id="1b4b5-127">Удаление объекта соглашения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-127">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="1b4b5-128">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b4b5-128">Properties</span></span>
| <span data-ttu-id="1b4b5-129">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b4b5-129">Property</span></span>     | <span data-ttu-id="1b4b5-130">Тип</span><span class="sxs-lookup"><span data-stu-id="1b4b5-130">Type</span></span>        | <span data-ttu-id="1b4b5-131">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4b5-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b4b5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="1b4b5-132">displayName</span></span>|<span data-ttu-id="1b4b5-133">Строка</span><span class="sxs-lookup"><span data-stu-id="1b4b5-133">String</span></span>|<span data-ttu-id="1b4b5-134">Отображаемое имя соглашения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="1b4b5-135">id</span><span class="sxs-lookup"><span data-stu-id="1b4b5-135">id</span></span>|<span data-ttu-id="1b4b5-136">Строка</span><span class="sxs-lookup"><span data-stu-id="1b4b5-136">String</span></span>| <span data-ttu-id="1b4b5-137">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-137">Read-only.</span></span>|
|<span data-ttu-id="1b4b5-138">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="1b4b5-138">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="1b4b5-139">Логический</span><span class="sxs-lookup"><span data-stu-id="1b4b5-139">Boolean</span></span>|<span data-ttu-id="1b4b5-140">Указывает, есть ли у пользователя можно развернуть и отобразить соглашения перед подтверждением.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-140">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b4b5-141">Связи</span><span class="sxs-lookup"><span data-stu-id="1b4b5-141">Relationships</span></span>
| <span data-ttu-id="1b4b5-142">Связь</span><span class="sxs-lookup"><span data-stu-id="1b4b5-142">Relationship</span></span> | <span data-ttu-id="1b4b5-143">Тип</span><span class="sxs-lookup"><span data-stu-id="1b4b5-143">Type</span></span>        | <span data-ttu-id="1b4b5-144">Описание</span><span class="sxs-lookup"><span data-stu-id="1b4b5-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1b4b5-145">files</span><span class="sxs-lookup"><span data-stu-id="1b4b5-145">files</span></span>|<span data-ttu-id="1b4b5-146">[agreementFile](agreementfile.md) коллекции</span><span class="sxs-lookup"><span data-stu-id="1b4b5-146">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="1b4b5-147">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-147">Read-only.</span></span> <span data-ttu-id="1b4b5-148">PDF-файлы, связанные с этого соглашения.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-148">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b4b5-149">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="1b4b5-149">JSON representation</span></span>

<span data-ttu-id="1b4b5-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b4b5-150">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
