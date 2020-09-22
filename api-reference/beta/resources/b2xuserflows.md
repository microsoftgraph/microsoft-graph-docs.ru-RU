---
title: Тип ресурса b2xUserFlows
description: Представляет пользовательский поток в клиенте Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 989fbb3e003acd4207740a300c1b6f5d0c926e08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089751"
---
# <a name="b2xuserflows-resource-type"></a><span data-ttu-id="98c04-103">Тип ресурса b2xUserFlows</span><span class="sxs-lookup"><span data-stu-id="98c04-103">b2xUserFlows resource type</span></span>

<span data-ttu-id="98c04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98c04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="98c04-105">Представляет пользовательский поток в клиенте Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="98c04-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="98c04-106">Пользовательские потоки используются для включения интерфейса [самостоятельной регистрации](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) для гостевых пользователей в приложении.</span><span class="sxs-lookup"><span data-stu-id="98c04-106">User flows are used to enable a [self-service sign up](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="98c04-107">Пользовательские потоки определяют интерфейс, демонстрируемый пользователям при регистрации, в том числе [поставщиков удостоверений](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers), которых они могут использовать для проверки подлинности, а также сведения о том, какие атрибуты собираются в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="98c04-107">User flows define the experience the end user sees while signing up, including which [identity providers](https://docs.microsoft.com/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="98c04-108">Методы</span><span class="sxs-lookup"><span data-stu-id="98c04-108">Methods</span></span>

| <span data-ttu-id="98c04-109">Метод</span><span class="sxs-lookup"><span data-stu-id="98c04-109">Method</span></span>       | <span data-ttu-id="98c04-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="98c04-110">Return Type</span></span>  |<span data-ttu-id="98c04-111">Описание</span><span class="sxs-lookup"><span data-stu-id="98c04-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="98c04-112">Перечисление пользовательских потоков</span><span class="sxs-lookup"><span data-stu-id="98c04-112">List user flows</span></span>](../api/b2xuserflows-list.md)|<span data-ttu-id="98c04-113">Коллекция b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="98c04-113">b2xUserFlow collection</span></span>|<span data-ttu-id="98c04-114">Извлечение всех пользовательских потоков.</span><span class="sxs-lookup"><span data-stu-id="98c04-114">Retrieve all user flows.</span></span>|
|[<span data-ttu-id="98c04-115">Получение пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="98c04-115">Get user flow</span></span>](../api/b2xuserflows-get.md)|<span data-ttu-id="98c04-116">b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="98c04-116">b2xUserFlow</span></span>|<span data-ttu-id="98c04-117">Извлечение свойств пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="98c04-117">Retrieve properties of a user flow.</span></span>|
|[<span data-ttu-id="98c04-118">Создание пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="98c04-118">Create user flow</span></span>](../api/b2xuserflow-post-b2xuserflows.md)|<span data-ttu-id="98c04-119">b2xUserFlow</span><span class="sxs-lookup"><span data-stu-id="98c04-119">b2xUserFlow</span></span>|<span data-ttu-id="98c04-120">Создание пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="98c04-120">Create a new user flow.</span></span>|
|[<span data-ttu-id="98c04-121">Удаление пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="98c04-121">Delete user flow</span></span>](../api/b2xuserflows-delete.md)|<span data-ttu-id="98c04-122">Нет</span><span class="sxs-lookup"><span data-stu-id="98c04-122">None</span></span>|<span data-ttu-id="98c04-123">Удаление пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="98c04-123">Delete a user flow.</span></span>|
|[<span data-ttu-id="98c04-124">Перечисление поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="98c04-124">List identity providers</span></span>](../api/b2xuserflows-list-identityproviders.md)|<span data-ttu-id="98c04-125">Коллекция объектов [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="98c04-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="98c04-126">Получение всех поставщиков удостоверений в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="98c04-126">Retrieve all identity providers in a user flow.</span></span>|
|[<span data-ttu-id="98c04-127">Добавление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="98c04-127">Add identity provider</span></span>](../api/b2xuserflows-update-identityprovider.md)|<span data-ttu-id="98c04-128">Нет</span><span class="sxs-lookup"><span data-stu-id="98c04-128">None</span></span>|<span data-ttu-id="98c04-129">Добавление поставщика удостоверений в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="98c04-129">Add an identity provider to a user flow.</span></span>|
|[<span data-ttu-id="98c04-130">Удаление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="98c04-130">Delete identity provider</span></span>](../api/b2xuserflows-delete-identityprovider.md)|<span data-ttu-id="98c04-131">Нет</span><span class="sxs-lookup"><span data-stu-id="98c04-131">None</span></span>|<span data-ttu-id="98c04-132">Удаление поставщика удостоверений из пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="98c04-132">Delete an identity provider from a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="98c04-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="98c04-133">Properties</span></span>

|<span data-ttu-id="98c04-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="98c04-134">Property</span></span>|<span data-ttu-id="98c04-135">Тип</span><span class="sxs-lookup"><span data-stu-id="98c04-135">Type</span></span>|<span data-ttu-id="98c04-136">Описание</span><span class="sxs-lookup"><span data-stu-id="98c04-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98c04-137">id</span><span class="sxs-lookup"><span data-stu-id="98c04-137">id</span></span>|<span data-ttu-id="98c04-138">Строка</span><span class="sxs-lookup"><span data-stu-id="98c04-138">String</span></span>|<span data-ttu-id="98c04-139">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="98c04-139">The name of the user flow.</span></span> <span data-ttu-id="98c04-140">Это обязательное значение, не изменяемое после создания.</span><span class="sxs-lookup"><span data-stu-id="98c04-140">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="98c04-141">После создания перед именем будет добавлен префикс со значением `B2X_1_`.</span><span class="sxs-lookup"><span data-stu-id="98c04-141">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="98c04-142">userFlowType</span><span class="sxs-lookup"><span data-stu-id="98c04-142">userFlowType</span></span>|<span data-ttu-id="98c04-143">Строка</span><span class="sxs-lookup"><span data-stu-id="98c04-143">String</span></span>|<span data-ttu-id="98c04-144">Тип пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="98c04-144">The type of user flow.</span></span> <span data-ttu-id="98c04-145">Для пользовательских потоков самостоятельной регистрации значением может быть только `signUpOrSignIn`, которое нельзя изменить после создания.</span><span class="sxs-lookup"><span data-stu-id="98c04-145">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="98c04-146">userFlowVersion</span><span class="sxs-lookup"><span data-stu-id="98c04-146">userFlowVersion</span></span>|<span data-ttu-id="98c04-147">Одинарное</span><span class="sxs-lookup"><span data-stu-id="98c04-147">Single</span></span>|<span data-ttu-id="98c04-148">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="98c04-148">The version of the user flow.</span></span> <span data-ttu-id="98c04-149">Для пользовательских потоков B2X всегда используется версия `1`.</span><span class="sxs-lookup"><span data-stu-id="98c04-149">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="98c04-150">Связи</span><span class="sxs-lookup"><span data-stu-id="98c04-150">Relationships</span></span>

| <span data-ttu-id="98c04-151">Связь</span><span class="sxs-lookup"><span data-stu-id="98c04-151">Relationship</span></span>       | <span data-ttu-id="98c04-152">Тип</span><span class="sxs-lookup"><span data-stu-id="98c04-152">Type</span></span>  |<span data-ttu-id="98c04-153">Описание</span><span class="sxs-lookup"><span data-stu-id="98c04-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="98c04-154">identityProviders</span><span class="sxs-lookup"><span data-stu-id="98c04-154">identityProviders</span></span>|<span data-ttu-id="98c04-155">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="98c04-155">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="98c04-156">Поставщики удостоверений, включенные в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="98c04-156">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="98c04-157">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="98c04-157">JSON representation</span></span>

<span data-ttu-id="98c04-158">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="98c04-158">The following is a JSON representation of the resource.</span></span>

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


