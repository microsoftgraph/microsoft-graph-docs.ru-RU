---
title: Тип ресурса b2xUserFlows
description: Представляет пользовательский поток в клиенте Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 8f25f99ec54f1db6b68bf5617518d90cc51d3ecc
ms.sourcegitcommit: 2c6e16dd8381945de6adf1eea020c142969b7801
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/01/2020
ms.locfileid: "47319826"
---
# <a name="b2xuserflows-resource-type"></a><span data-ttu-id="a8e63-103">Тип ресурса b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="a8e63-103">b2xUserFlows resource type</span></span>

<span data-ttu-id="a8e63-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8e63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8e63-105">Представляет пользовательский поток в клиенте Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a8e63-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="a8e63-106">Пользовательские потоки используются для включения интерфейса [самостоятельной регистрации](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) для гостевых пользователей в приложении.</span><span class="sxs-lookup"><span data-stu-id="a8e63-106">User flows are used to enable a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="a8e63-107">Пользовательские потоки определяют интерфейс, демонстрируемый пользователям при регистрации, в том числе [поставщиков удостоверений](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers), которых они могут использовать для проверки подлинности, а также сведения о том, какие атрибуты собираются в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="a8e63-107">User flows define the experience the end user sees while signing up, including which [identity providers](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="a8e63-108">Методы</span><span class="sxs-lookup"><span data-stu-id="a8e63-108">Methods</span></span>

| <span data-ttu-id="a8e63-109">Метод</span><span class="sxs-lookup"><span data-stu-id="a8e63-109">Method</span></span>       | <span data-ttu-id="a8e63-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="a8e63-110">Return Type</span></span>  |<span data-ttu-id="a8e63-111">Описание</span><span class="sxs-lookup"><span data-stu-id="a8e63-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8e63-112">Перечисление пользовательских потоков</span><span class="sxs-lookup"><span data-stu-id="a8e63-112">List user flows</span></span>](../api/b2xuserflows-list.md)|<span data-ttu-id="a8e63-113">Коллекция b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="a8e63-113">b2xUserFlow collection</span></span>|<span data-ttu-id="a8e63-114">Извлечение всех пользовательских потоков.</span><span class="sxs-lookup"><span data-stu-id="a8e63-114">Retrieve all user flows.</span></span>|
|[<span data-ttu-id="a8e63-115">Получение пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="a8e63-115">Get user flow</span></span>](../api/b2xuserflows-get.md)|<span data-ttu-id="a8e63-116">b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="a8e63-116">b2xUserFlow</span></span>|<span data-ttu-id="a8e63-117">Извлечение свойств пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a8e63-117">Retrieve properties of a user flow.</span></span>|
|[<span data-ttu-id="a8e63-118">Создание пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="a8e63-118">Create user flow</span></span>](../api/b2xuserflow-post-b2xuserflows.md)|<span data-ttu-id="a8e63-119">b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="a8e63-119">b2xUserFlow</span></span>|<span data-ttu-id="a8e63-120">Создание пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a8e63-120">Create a new user flow.</span></span>|
|[<span data-ttu-id="a8e63-121">Удаление пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="a8e63-121">Delete user flow</span></span>](../api/b2xuserflows-delete.md)|<span data-ttu-id="a8e63-122">Нет</span><span class="sxs-lookup"><span data-stu-id="a8e63-122">None</span></span>|<span data-ttu-id="a8e63-123">Удаление пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a8e63-123">Delete a user flow.</span></span>|
|[<span data-ttu-id="a8e63-124">Перечисление поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="a8e63-124">List identity providers</span></span>](../api/b2xuserflows-list-identityproviders.md)|<span data-ttu-id="a8e63-125">Коллекция объектов [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="a8e63-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="a8e63-126">Получение всех поставщиков удостоверений в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="a8e63-126">Retrieve all identity providers in a user flow.</span></span>|
|[<span data-ttu-id="a8e63-127">Добавление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="a8e63-127">Add identity provider</span></span>](../api/b2xuserflows-update-identityprovider.md)|<span data-ttu-id="a8e63-128">Нет</span><span class="sxs-lookup"><span data-stu-id="a8e63-128">None</span></span>|<span data-ttu-id="a8e63-129">Добавление поставщика удостоверений в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="a8e63-129">Add an identity provider to a user flow.</span></span>|
|[<span data-ttu-id="a8e63-130">Удаление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="a8e63-130">Delete identity provider</span></span>](../api/b2xuserflows-delete-identityprovider.md)|<span data-ttu-id="a8e63-131">Нет</span><span class="sxs-lookup"><span data-stu-id="a8e63-131">None</span></span>|<span data-ttu-id="a8e63-132">Удаление поставщика удостоверений из пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a8e63-132">Delete an identity provider from a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8e63-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="a8e63-133">Properties</span></span>

|<span data-ttu-id="a8e63-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="a8e63-134">Property</span></span>|<span data-ttu-id="a8e63-135">Тип</span><span class="sxs-lookup"><span data-stu-id="a8e63-135">Type</span></span>|<span data-ttu-id="a8e63-136">Описание</span><span class="sxs-lookup"><span data-stu-id="a8e63-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8e63-137">id</span><span class="sxs-lookup"><span data-stu-id="a8e63-137">id</span></span>|<span data-ttu-id="a8e63-138">Строка</span><span class="sxs-lookup"><span data-stu-id="a8e63-138">String</span></span>|<span data-ttu-id="a8e63-139">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a8e63-139">The name of the user flow.</span></span> <span data-ttu-id="a8e63-140">Это обязательное значение, не изменяемое после создания.</span><span class="sxs-lookup"><span data-stu-id="a8e63-140">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="a8e63-141">После создания перед именем будет добавлен префикс со значением `B2X_1_`.</span><span class="sxs-lookup"><span data-stu-id="a8e63-141">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="a8e63-142">userFlowType</span><span class="sxs-lookup"><span data-stu-id="a8e63-142">userFlowType</span></span>|<span data-ttu-id="a8e63-143">Строка</span><span class="sxs-lookup"><span data-stu-id="a8e63-143">String</span></span>|<span data-ttu-id="a8e63-144">Тип пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a8e63-144">The type of user flow.</span></span> <span data-ttu-id="a8e63-145">Для пользовательских потоков самостоятельной регистрации значением может быть только `signUpOrSignIn`, которое нельзя изменить после создания.</span><span class="sxs-lookup"><span data-stu-id="a8e63-145">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="a8e63-146">userFlowVersion</span><span class="sxs-lookup"><span data-stu-id="a8e63-146">userFlowVersion</span></span>|<span data-ttu-id="a8e63-147">Одинарное</span><span class="sxs-lookup"><span data-stu-id="a8e63-147">Single</span></span>|<span data-ttu-id="a8e63-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="a8e63-148">The version of the user flow.</span></span> <span data-ttu-id="a8e63-149">Для пользовательских потоков B2X всегда используется версия `1`.</span><span class="sxs-lookup"><span data-stu-id="a8e63-149">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8e63-150">Связи</span><span class="sxs-lookup"><span data-stu-id="a8e63-150">Relationships</span></span>

| <span data-ttu-id="a8e63-151">Связь</span><span class="sxs-lookup"><span data-stu-id="a8e63-151">Relationship</span></span>       | <span data-ttu-id="a8e63-152">Тип</span><span class="sxs-lookup"><span data-stu-id="a8e63-152">Type</span></span>  |<span data-ttu-id="a8e63-153">Описание</span><span class="sxs-lookup"><span data-stu-id="a8e63-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8e63-154">identityProviders</span><span class="sxs-lookup"><span data-stu-id="a8e63-154">identityProviders</span></span>|<span data-ttu-id="a8e63-155">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="a8e63-155">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="a8e63-156">Поставщики удостоверений, включенные в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="a8e63-156">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8e63-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a8e63-157">JSON representation</span></span>

<span data-ttu-id="a8e63-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a8e63-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2xIdentityUserFlow",
  "optionalProperties": [],
  "keyProperty": "id"
} -->

```json
{
    "id": "String (identifier)",
    "userFlowType": "String",
    "userFlowTypeVersion": "Single",
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```
