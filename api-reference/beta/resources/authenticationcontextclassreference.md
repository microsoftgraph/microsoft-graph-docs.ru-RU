---
title: тип ресурса authenticationContextClassReference
description: Представляет ссылку Azure Active Directory класса проверки подлинности.
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1397545d7b102d05b8c71957cea88f9c131f0e09
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547534"
---
# <a name="authenticationcontextclassreference-resource-type"></a><span data-ttu-id="5d89c-103">тип ресурса authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="5d89c-103">authenticationContextClassReference resource type</span></span>

<span data-ttu-id="5d89c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d89c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5d89c-105">Представляет ссылку Azure Active Directory класса проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5d89c-105">Represents an Azure Active Directory authentication context class reference.</span></span> <span data-ttu-id="5d89c-106">Ссылки на класс контекста проверки подлинности — это настраиваемые значения, которые определяют требование проверки подлинности условного доступа.</span><span class="sxs-lookup"><span data-stu-id="5d89c-106">Authentication context class references are custom values that define a Conditional Access authentication requirement.</span></span>

## <a name="methods"></a><span data-ttu-id="5d89c-107">Методы</span><span class="sxs-lookup"><span data-stu-id="5d89c-107">Methods</span></span>

| <span data-ttu-id="5d89c-108">Метод</span><span class="sxs-lookup"><span data-stu-id="5d89c-108">Method</span></span>       | <span data-ttu-id="5d89c-109">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="5d89c-109">Return Type</span></span> | <span data-ttu-id="5d89c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5d89c-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="5d89c-111">Проверка подлинности спискаContextClassReference</span><span class="sxs-lookup"><span data-stu-id="5d89c-111">List authenticationContextClassReference</span></span>](../api/conditionalaccessroot-list-authenticationcontextclassreferences.md) | <span data-ttu-id="5d89c-112">[коллекция authenticationContextClassReference](authenticationContextClassReference.md)</span><span class="sxs-lookup"><span data-stu-id="5d89c-112">[authenticationContextClassReference](authenticationContextClassReference.md) collection</span></span> | <span data-ttu-id="5d89c-113">Получите все объекты authenticationContextClassReference в организации.</span><span class="sxs-lookup"><span data-stu-id="5d89c-113">Get all of the authenticationContextClassReference objects in the organization.</span></span> |
| [<span data-ttu-id="5d89c-114">Создание проверки подлинностиContextClassReference</span><span class="sxs-lookup"><span data-stu-id="5d89c-114">Create authenticationContextClassReference</span></span>](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md) | [<span data-ttu-id="5d89c-115">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="5d89c-115">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="5d89c-116">Создание нового объекта проверки подлинностиContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="5d89c-116">Create a new authenticationContextClassReference object.</span></span> |
| [<span data-ttu-id="5d89c-117">Проверка подлинностиContextClassReference</span><span class="sxs-lookup"><span data-stu-id="5d89c-117">Get authenticationContextClassReference</span></span>](../api/authenticationcontextclassreference-get.md) | [<span data-ttu-id="5d89c-118">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="5d89c-118">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="5d89c-119">Чтение свойств и связей объекта authenticationContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="5d89c-119">Read properties and relationships of a authenticationContextClassReference object.</span></span> |
| [<span data-ttu-id="5d89c-120">Обновление проверки подлинностиContextClassReference</span><span class="sxs-lookup"><span data-stu-id="5d89c-120">Update authenticationContextClassReference</span></span>](../api/authenticationcontextclassreference-update.md) | [<span data-ttu-id="5d89c-121">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="5d89c-121">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="5d89c-122">Обновление объекта authenticationContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="5d89c-122">Update a authenticationContextClassReference object.</span></span> |


## <a name="properties"></a><span data-ttu-id="5d89c-123">Свойства</span><span class="sxs-lookup"><span data-stu-id="5d89c-123">Properties</span></span>

| <span data-ttu-id="5d89c-124">Свойство</span><span class="sxs-lookup"><span data-stu-id="5d89c-124">Property</span></span>     | <span data-ttu-id="5d89c-125">Тип</span><span class="sxs-lookup"><span data-stu-id="5d89c-125">Type</span></span>        | <span data-ttu-id="5d89c-126">Описание</span><span class="sxs-lookup"><span data-stu-id="5d89c-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5d89c-127">id</span><span class="sxs-lookup"><span data-stu-id="5d89c-127">id</span></span>|<span data-ttu-id="5d89c-128">String</span><span class="sxs-lookup"><span data-stu-id="5d89c-128">String</span></span>| <span data-ttu-id="5d89c-129">Идентификатор, используемый для ссылки на класс контекста проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5d89c-129">Identifier used to reference the authentication context class.</span></span> <span data-ttu-id="5d89c-130">ID используется для запуска этапной проверки подлинности для ссылаемого требования к проверке подлинности и является значением, которое будет выдано в утверждении acrs.</span><span class="sxs-lookup"><span data-stu-id="5d89c-130">The id is used to trigger step-up authentication for the referenced authentication requirements and is the value that will be issued in the acrs claim.</span></span> <span data-ttu-id="5d89c-131">Это значение в утверждении используется для проверки удовлетворенности необходимого контекста проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="5d89c-131">This value in the claim is used to verify the required authentication context has been satisfied.</span></span> <span data-ttu-id="5d89c-132">Допустимые значения id — это "c1" через "c25".</span><span class="sxs-lookup"><span data-stu-id="5d89c-132">The allowed id values are "c1" through "c25".</span></span> |
|<span data-ttu-id="5d89c-133">displayName</span><span class="sxs-lookup"><span data-stu-id="5d89c-133">displayName</span></span>|<span data-ttu-id="5d89c-134">String</span><span class="sxs-lookup"><span data-stu-id="5d89c-134">String</span></span>| <span data-ttu-id="5d89c-135">Имя отображения — это удобное имя проверки подлинностиContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="5d89c-135">The display name is the friendly name of the authenticationContextClassReference.</span></span> <span data-ttu-id="5d89c-136">Это значение следует использовать для определения ссылки класса контекста проверки подлинности при создании пользовательских интерфейсов администратора.</span><span class="sxs-lookup"><span data-stu-id="5d89c-136">This value should be used to identify the authentication context class reference when building user facing admin experiences.</span></span> <span data-ttu-id="5d89c-137">Например, выбор UX.</span><span class="sxs-lookup"><span data-stu-id="5d89c-137">For example, selection UX.</span></span> |
|<span data-ttu-id="5d89c-138">description</span><span class="sxs-lookup"><span data-stu-id="5d89c-138">description</span></span>|<span data-ttu-id="5d89c-139">String</span><span class="sxs-lookup"><span data-stu-id="5d89c-139">String</span></span>| <span data-ttu-id="5d89c-140">Краткое объяснение политик, которые применяются при проверке подлинностиContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="5d89c-140">A short explanation of the policies that are enforced by authenticationContextClassReference.</span></span> <span data-ttu-id="5d89c-141">Это значение следует использовать для предоставления дополнительного текста для описания ссылки класса контекста проверки подлинности при создании пользовательских интерфейсов администратора.</span><span class="sxs-lookup"><span data-stu-id="5d89c-141">This value should be used to provide secondary text to describe the authentication context class reference when building user facing admin experiences.</span></span> <span data-ttu-id="5d89c-142">Например, выбор UX.</span><span class="sxs-lookup"><span data-stu-id="5d89c-142">For example, selection UX.</span></span>|
|<span data-ttu-id="5d89c-143">isAvailable</span><span class="sxs-lookup"><span data-stu-id="5d89c-143">isAvailable</span></span>|<span data-ttu-id="5d89c-144">boolean</span><span class="sxs-lookup"><span data-stu-id="5d89c-144">boolean</span></span>| <span data-ttu-id="5d89c-145">Указывает, была ли проверка подлинностиContextClassReference опубликована администратором безопасности и готова к использованию приложениями.</span><span class="sxs-lookup"><span data-stu-id="5d89c-145">Indicates whether the authenticationContextClassReference has been published by the security admin and is ready for use by apps.</span></span> <span data-ttu-id="5d89c-146">Если она установлена, ее не следует показывать в интерфейсе администрирования, так как в настоящее время значение не доступно `false` для выбора.</span><span class="sxs-lookup"><span data-stu-id="5d89c-146">When it is set to `false` it should not be shown in admin UX experiences because the value is not currently available for selection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5d89c-147">Связи</span><span class="sxs-lookup"><span data-stu-id="5d89c-147">Relationships</span></span>

<span data-ttu-id="5d89c-148">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="5d89c-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5d89c-149">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="5d89c-149">JSON representation</span></span>

<span data-ttu-id="5d89c-150">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="5d89c-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
    {
      "id": "String",
      "displayName": "String",
      "description": "String",
      "isAvailable": "boolean",
    }

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationContextClassReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
