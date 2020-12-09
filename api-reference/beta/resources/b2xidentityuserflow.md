---
title: Тип ресурса b2xIdentityUserFlow
description: Представляет пользовательский поток в клиенте Azure Active Directory.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: e1051d60681e42012fd9df3fd8655a9e4cc745cd
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49580965"
---
# <a name="b2xidentityuserflow-resource-type"></a><span data-ttu-id="52b4e-103">Тип ресурса b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="52b4e-103">b2xIdentityUserFlow resource type</span></span>

<span data-ttu-id="52b4e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52b4e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52b4e-105">Представляет пользовательский поток в клиенте Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52b4e-105">Represents a user flow within an Azure Active Directory tenant.</span></span>

<span data-ttu-id="52b4e-106">Пользовательские потоки используются для включения интерфейса [самостоятельной регистрации](/azure/active-directory/external-identities/self-service-sign-up-overview) для гостевых пользователей в приложении.</span><span class="sxs-lookup"><span data-stu-id="52b4e-106">User flows are used to enable a [self-service sign up](/azure/active-directory/external-identities/self-service-sign-up-overview) experience for guest users on an application.</span></span> <span data-ttu-id="52b4e-107">Пользовательские потоки определяют интерфейс, демонстрируемый пользователям при регистрации, в том числе [поставщиков удостоверений](/azure/active-directory/external-identities/identity-providers), которых они могут использовать для проверки подлинности, а также сведения о том, какие атрибуты собираются в процессе регистрации.</span><span class="sxs-lookup"><span data-stu-id="52b4e-107">User flows define the experience the end user sees while signing up, including which [identity providers](/azure/active-directory/external-identities/identity-providers) they can use to authenticate, along with which attributes are collected as part of the sign up process.</span></span>

## <a name="methods"></a><span data-ttu-id="52b4e-108">Методы</span><span class="sxs-lookup"><span data-stu-id="52b4e-108">Methods</span></span>

| <span data-ttu-id="52b4e-109">Метод</span><span class="sxs-lookup"><span data-stu-id="52b4e-109">Method</span></span>       | <span data-ttu-id="52b4e-110">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="52b4e-110">Return Type</span></span>  |<span data-ttu-id="52b4e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="52b4e-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52b4e-112">Перечисление пользовательских потоков</span><span class="sxs-lookup"><span data-stu-id="52b4e-112">List user flows</span></span>](../api/identitycontainer-list-b2xuserflows.md)|<span data-ttu-id="52b4e-113">Коллекция b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="52b4e-113">b2xIdentityUserFlow collection</span></span>|<span data-ttu-id="52b4e-114">Извлечение всех пользовательских потоков B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-114">Retrieve all B2X user flows.</span></span>|
|[<span data-ttu-id="52b4e-115">Получение пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="52b4e-115">Get user flow</span></span>](../api/b2xidentityuserflow-get.md)|<span data-ttu-id="52b4e-116">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="52b4e-116">b2xIdentityUserFlow</span></span>|<span data-ttu-id="52b4e-117">Извлечение свойств пользовательского потока B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-117">Retrieve properties of a B2X user flow.</span></span>|
|[<span data-ttu-id="52b4e-118">Создание пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="52b4e-118">Create user flow</span></span>](../api/identitycontainer-post-b2xuserflows.md)|<span data-ttu-id="52b4e-119">b2xIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="52b4e-119">b2xIdentityUserFlow</span></span>|<span data-ttu-id="52b4e-120">Создание пользовательского потока B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-120">Create a new B2X user flow.</span></span>|
|[<span data-ttu-id="52b4e-121">Удаление пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="52b4e-121">Delete user flow</span></span>](../api/b2xidentityuserflow-delete.md)|<span data-ttu-id="52b4e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="52b4e-122">None</span></span>|<span data-ttu-id="52b4e-123">Удаление пользовательского потока B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-123">Delete a B2X user flow.</span></span>|
|[<span data-ttu-id="52b4e-124">Перечисление поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="52b4e-124">List identity providers</span></span>](../api/b2xidentityuserflow-list-identityproviders.md)|<span data-ttu-id="52b4e-125">Коллекция объектов [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="52b4e-125">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="52b4e-126">Получение всех поставщиков удостоверений в пользовательском потоке B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-126">Retrieve all identity providers in a B2X user flow.</span></span>|
|[<span data-ttu-id="52b4e-127">Добавление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="52b4e-127">Add identity provider</span></span>](../api/b2xidentityuserflow-post-identityproviders.md)|<span data-ttu-id="52b4e-128">Нет</span><span class="sxs-lookup"><span data-stu-id="52b4e-128">None</span></span>|<span data-ttu-id="52b4e-129">Добавление поставщика удостоверений в пользовательский поток B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-129">Add an identity provider to a B2X user flow.</span></span>|
|[<span data-ttu-id="52b4e-130">Удаление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="52b4e-130">Remove identity provider</span></span>](../api/b2xidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="52b4e-131">Нет</span><span class="sxs-lookup"><span data-stu-id="52b4e-131">None</span></span>|<span data-ttu-id="52b4e-132">Удаление поставщика удостоверений из пользовательского потока B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-132">Remove an identity provider from a B2X user flow.</span></span>|
|[<span data-ttu-id="52b4e-133">Назначения атрибутов пользователя в списке</span><span class="sxs-lookup"><span data-stu-id="52b4e-133">List user attribute assignments</span></span>](../api/b2xidentityuserflow-list-userattributeassignments.md)|<span data-ttu-id="52b4e-134">Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="52b4e-134">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="52b4e-135">Извлечение всех назначений атрибутов пользователя в потоке пользователей B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-135">Retrieve all user attribute assignments in a B2X user flow.</span></span>|
|[<span data-ttu-id="52b4e-136">Создание назначения атрибута пользователя</span><span class="sxs-lookup"><span data-stu-id="52b4e-136">Create user attribute assignment</span></span>](../api/b2xidentityuserflow-post-userattributeassignments.md)|[<span data-ttu-id="52b4e-137">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="52b4e-137">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="52b4e-138">Создание назначения атрибута пользователя в потоке пользователей B2X.</span><span class="sxs-lookup"><span data-stu-id="52b4e-138">Create a user attribute assignment in a B2X user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="52b4e-139">Свойства</span><span class="sxs-lookup"><span data-stu-id="52b4e-139">Properties</span></span>

|<span data-ttu-id="52b4e-140">Свойство</span><span class="sxs-lookup"><span data-stu-id="52b4e-140">Property</span></span>|<span data-ttu-id="52b4e-141">Тип</span><span class="sxs-lookup"><span data-stu-id="52b4e-141">Type</span></span>|<span data-ttu-id="52b4e-142">Описание</span><span class="sxs-lookup"><span data-stu-id="52b4e-142">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52b4e-143">id</span><span class="sxs-lookup"><span data-stu-id="52b4e-143">id</span></span>|<span data-ttu-id="52b4e-144">Строка</span><span class="sxs-lookup"><span data-stu-id="52b4e-144">String</span></span>|<span data-ttu-id="52b4e-145">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="52b4e-145">The name of the user flow.</span></span> <span data-ttu-id="52b4e-146">Это обязательное значение, не изменяемое после создания.</span><span class="sxs-lookup"><span data-stu-id="52b4e-146">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="52b4e-147">После создания перед именем будет добавлен префикс со значением `B2X_1_`.</span><span class="sxs-lookup"><span data-stu-id="52b4e-147">The name will be prefixed with the value of `B2X_1_` after creation.</span></span>|
|<span data-ttu-id="52b4e-148">userFlowType</span><span class="sxs-lookup"><span data-stu-id="52b4e-148">userFlowType</span></span>|<span data-ttu-id="52b4e-149">Строка</span><span class="sxs-lookup"><span data-stu-id="52b4e-149">String</span></span>|<span data-ttu-id="52b4e-150">Тип пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="52b4e-150">The type of user flow.</span></span> <span data-ttu-id="52b4e-151">Для пользовательских потоков самостоятельной регистрации значением может быть только `signUpOrSignIn`, которое нельзя изменить после создания.</span><span class="sxs-lookup"><span data-stu-id="52b4e-151">For self-service sign up user flows, the value can only be `signUpOrSignIn` and cannot be modified after creation.</span></span>|
|<span data-ttu-id="52b4e-152">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="52b4e-152">userFlowTypeVersion</span></span>|<span data-ttu-id="52b4e-153">Одинарное</span><span class="sxs-lookup"><span data-stu-id="52b4e-153">Single</span></span>|<span data-ttu-id="52b4e-154">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="52b4e-154">The version of the user flow.</span></span> <span data-ttu-id="52b4e-155">Для пользовательских потоков B2X всегда используется версия `1`.</span><span class="sxs-lookup"><span data-stu-id="52b4e-155">For B2X user flows, the version is always `1`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52b4e-156">Связи</span><span class="sxs-lookup"><span data-stu-id="52b4e-156">Relationships</span></span>

| <span data-ttu-id="52b4e-157">Связь</span><span class="sxs-lookup"><span data-stu-id="52b4e-157">Relationship</span></span>       | <span data-ttu-id="52b4e-158">Тип</span><span class="sxs-lookup"><span data-stu-id="52b4e-158">Type</span></span>  |<span data-ttu-id="52b4e-159">Описание</span><span class="sxs-lookup"><span data-stu-id="52b4e-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52b4e-160">identityProviders</span><span class="sxs-lookup"><span data-stu-id="52b4e-160">identityProviders</span></span>|<span data-ttu-id="52b4e-161">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="52b4e-161">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="52b4e-162">Поставщики удостоверений, включенные в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="52b4e-162">The identity providers included in the user flow.</span></span>|
|<span data-ttu-id="52b4e-163">userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="52b4e-163">userAttributeAssignments</span></span>|<span data-ttu-id="52b4e-164">Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="52b4e-164">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="52b4e-165">Назначения атрибутов пользователя, включенные в поток пользователей.</span><span class="sxs-lookup"><span data-stu-id="52b4e-165">The user attribute assignments included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52b4e-166">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="52b4e-166">JSON representation</span></span>

<span data-ttu-id="52b4e-167">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="52b4e-167">The following is a JSON representation of the resource.</span></span>

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}],
    "userAttributeAssignments": [{"@odate.type": "microsoft.graph.identityUserFlowAttributeAssignment"}]
}
```
