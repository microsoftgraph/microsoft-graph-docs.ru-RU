---
title: Тип ресурса b2cIdentityUserFlow
description: Представляет пользовательский поток в клиенте Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 61c3a206ee07eb7e8474e501f9064a20c6cc3840
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581091"
---
# <a name="b2cidentityuserflow-resource-type"></a><span data-ttu-id="eab6a-103">Тип ресурса b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="eab6a-103">b2cIdentityUserFlow resource type</span></span>

<span data-ttu-id="eab6a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eab6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eab6a-105">Представляет пользовательский поток в клиенте Azure Active Directory B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-105">Represents a user flow within an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="eab6a-106">Чтобы помочь с настройкой наиболее распространенных задач идентификации для ваших приложений, Azure Active Directory B2C содержит заранее определенные настраиваемые политики, называемые [пользовательскими потоками](/azure/active-directory-b2c/user-flow-overview).</span><span class="sxs-lookup"><span data-stu-id="eab6a-106">To help you set up the most common identity tasks for your applications, Azure Active Directory B2C includes predefined, configurable policies called [user flows](/azure/active-directory-b2c/user-flow-overview).</span></span> <span data-ttu-id="eab6a-107">Пользовательский поток позволяет вам определить, как пользователи взаимодействуют с вашим приложением, когда они выполняют такие задачи, как вход, регистрация, изменение профиля или сброс пароля.</span><span class="sxs-lookup"><span data-stu-id="eab6a-107">A user flow lets you determine how users interact with your application when they do things like sign in, sign up, edit a profile, or reset a password.</span></span> <span data-ttu-id="eab6a-108">Вы можете создать множество пользовательских потоков различных типов в своем клиенте и использовать их в приложении по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="eab6a-108">You can create many user flows of different types in your tenant and use them in your applications as needed.</span></span> <span data-ttu-id="eab6a-109">С помощью пользовательских потоков вы можете управлять следующими возможностями:</span><span class="sxs-lookup"><span data-stu-id="eab6a-109">With user flows, you can control the following capabilities:</span></span>

- <span data-ttu-id="eab6a-110">Типы учетных записей, используемые для входа, например учетные записи социальных сетей, таких как Facebook, или локальные учетные записи</span><span class="sxs-lookup"><span data-stu-id="eab6a-110">Account types used for sign-in, such as social accounts like a Facebook or local account</span></span>
- <span data-ttu-id="eab6a-111">Атрибуты, собираемые у пользователей, такие как имя, почтовый индекс и размер обуви</span><span class="sxs-lookup"><span data-stu-id="eab6a-111">Attributes to be collected from the consumer, such as first name, postal code, and shoe size</span></span>
- <span data-ttu-id="eab6a-112">Многофакторная проверка подлинности Azure</span><span class="sxs-lookup"><span data-stu-id="eab6a-112">Azure Multi-Factor Authentication</span></span>
- <span data-ttu-id="eab6a-113">Настройка пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="eab6a-113">Customization of the user interface</span></span>
- <span data-ttu-id="eab6a-114">Сведения, получаемые приложением в маркере</span><span class="sxs-lookup"><span data-stu-id="eab6a-114">Information that the application receives in the token</span></span>

## <a name="methods"></a><span data-ttu-id="eab6a-115">Методы</span><span class="sxs-lookup"><span data-stu-id="eab6a-115">Methods</span></span>

| <span data-ttu-id="eab6a-116">Метод</span><span class="sxs-lookup"><span data-stu-id="eab6a-116">Method</span></span>       | <span data-ttu-id="eab6a-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="eab6a-117">Return Type</span></span>  |<span data-ttu-id="eab6a-118">Описание</span><span class="sxs-lookup"><span data-stu-id="eab6a-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="eab6a-119">Перечисление пользовательских потоков</span><span class="sxs-lookup"><span data-stu-id="eab6a-119">List user flows</span></span>](../api/identitycontainer-list-b2cuserflows.md)|<span data-ttu-id="eab6a-120">Коллекция b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="eab6a-120">b2cIdentityUserFlow collection</span></span>|<span data-ttu-id="eab6a-121">Извлечение всех пользовательских потоков B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-121">Retrieve all B2C user flows.</span></span>|
|[<span data-ttu-id="eab6a-122">Получение пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="eab6a-122">Get user flow</span></span>](../api/b2cidentityuserflow-get.md)|<span data-ttu-id="eab6a-123">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="eab6a-123">b2cIdentityUserFlow</span></span>|<span data-ttu-id="eab6a-124">Извлечение свойств пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-124">Retrieve properties of a B2C user flow.</span></span>|
|[<span data-ttu-id="eab6a-125">Создание пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="eab6a-125">Create user flow</span></span>](../api/identitycontainer-post-b2cuserflows.md)|<span data-ttu-id="eab6a-126">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="eab6a-126">b2cIdentityUserFlow</span></span>|<span data-ttu-id="eab6a-127">Создание пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-127">Create a new B2C user flow.</span></span>|
|[<span data-ttu-id="eab6a-128">Удаление пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="eab6a-128">Delete user flow</span></span>](../api/b2cidentityuserflow-delete.md)|<span data-ttu-id="eab6a-129">Нет</span><span class="sxs-lookup"><span data-stu-id="eab6a-129">None</span></span>|<span data-ttu-id="eab6a-130">Удаление пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-130">Delete a B2C user flow.</span></span>|
|[<span data-ttu-id="eab6a-131">Перечисление поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="eab6a-131">List identity providers</span></span>](../api/b2cidentityuserflow-list-identityproviders.md)|<span data-ttu-id="eab6a-132">Коллекция объектов [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="eab6a-132">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="eab6a-133">Получение всех поставщиков удостоверений в пользовательском потоке B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-133">Retrieve all identity providers in a B2C user flow.</span></span>|
|[<span data-ttu-id="eab6a-134">Добавление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="eab6a-134">Add identity provider</span></span>](../api/b2cidentityuserflow-post-identityproviders.md)|<span data-ttu-id="eab6a-135">Нет</span><span class="sxs-lookup"><span data-stu-id="eab6a-135">None</span></span>|<span data-ttu-id="eab6a-136">Добавление поставщика удостоверений в пользовательский поток B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-136">Add an identity provider to a B2C user flow.</span></span>|
|[<span data-ttu-id="eab6a-137">Удаление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="eab6a-137">Remove identity provider</span></span>](../api/b2cidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="eab6a-138">Нет</span><span class="sxs-lookup"><span data-stu-id="eab6a-138">None</span></span>|<span data-ttu-id="eab6a-139">Удаление поставщика удостоверений из пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-139">Remove an identity provider from a B2C user flow.</span></span>|
|[<span data-ttu-id="eab6a-140">Назначения атрибутов пользователя в списке</span><span class="sxs-lookup"><span data-stu-id="eab6a-140">List user attribute assignments</span></span>](../api/b2cidentityuserflow-list-userattributeassignments.md)|<span data-ttu-id="eab6a-141">Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eab6a-141">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="eab6a-142">Извлечение всех назначений атрибутов пользователя в потоке пользователей B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-142">Retrieve all user attribute assignments in a B2C user flow.</span></span>|
|[<span data-ttu-id="eab6a-143">Создание назначения атрибута пользователя</span><span class="sxs-lookup"><span data-stu-id="eab6a-143">Create user attribute assignment</span></span>](../api/b2cidentityuserflow-post-userattributeassignments.md)|[<span data-ttu-id="eab6a-144">identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="eab6a-144">identityUserFlowAttributeAssignment</span></span>](../resources/identityuserflowattributeassignment.md)|<span data-ttu-id="eab6a-145">Создание назначения атрибута пользователя в потоке пользователей B2C.</span><span class="sxs-lookup"><span data-stu-id="eab6a-145">Create a user attribute assignment in a B2C user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="eab6a-146">Свойства</span><span class="sxs-lookup"><span data-stu-id="eab6a-146">Properties</span></span>

|<span data-ttu-id="eab6a-147">Свойство</span><span class="sxs-lookup"><span data-stu-id="eab6a-147">Property</span></span>|<span data-ttu-id="eab6a-148">Тип</span><span class="sxs-lookup"><span data-stu-id="eab6a-148">Type</span></span>|<span data-ttu-id="eab6a-149">Описание</span><span class="sxs-lookup"><span data-stu-id="eab6a-149">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eab6a-150">id</span><span class="sxs-lookup"><span data-stu-id="eab6a-150">id</span></span>|<span data-ttu-id="eab6a-151">Строка</span><span class="sxs-lookup"><span data-stu-id="eab6a-151">String</span></span>|<span data-ttu-id="eab6a-152">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="eab6a-152">The name of the user flow.</span></span> <span data-ttu-id="eab6a-153">Это обязательное значение, не изменяемое после создания.</span><span class="sxs-lookup"><span data-stu-id="eab6a-153">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="eab6a-154">После создания перед именем будет добавлен префикс со значением `B2C_1_`.</span><span class="sxs-lookup"><span data-stu-id="eab6a-154">The name will be prefixed with the value of `B2C_1_` after creation.</span></span>|
|<span data-ttu-id="eab6a-155">userFlowType</span><span class="sxs-lookup"><span data-stu-id="eab6a-155">userFlowType</span></span>|<span data-ttu-id="eab6a-156">Строка</span><span class="sxs-lookup"><span data-stu-id="eab6a-156">String</span></span>|<span data-ttu-id="eab6a-157">[Тип пользовательского потока](/azure/active-directory-b2c/user-flow-versions).</span><span class="sxs-lookup"><span data-stu-id="eab6a-157">The [type of user flow](/azure/active-directory-b2c/user-flow-versions).</span></span> <span data-ttu-id="eab6a-158">Поддерживаемые значения для **userFlowType**:</span><span class="sxs-lookup"><span data-stu-id="eab6a-158">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwner`</li>|
|<span data-ttu-id="eab6a-159">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="eab6a-159">userFlowTypeVersion</span></span>|<span data-ttu-id="eab6a-160">Одинарное</span><span class="sxs-lookup"><span data-stu-id="eab6a-160">Single</span></span>|<span data-ttu-id="eab6a-161">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="eab6a-161">The version of the user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eab6a-162">Связи</span><span class="sxs-lookup"><span data-stu-id="eab6a-162">Relationships</span></span>

| <span data-ttu-id="eab6a-163">Связь</span><span class="sxs-lookup"><span data-stu-id="eab6a-163">Relationship</span></span>       | <span data-ttu-id="eab6a-164">Тип</span><span class="sxs-lookup"><span data-stu-id="eab6a-164">Type</span></span>  |<span data-ttu-id="eab6a-165">Описание</span><span class="sxs-lookup"><span data-stu-id="eab6a-165">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eab6a-166">identityProviders</span><span class="sxs-lookup"><span data-stu-id="eab6a-166">identityProviders</span></span>|<span data-ttu-id="eab6a-167">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="eab6a-167">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="eab6a-168">Поставщики удостоверений, включенные в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="eab6a-168">The identity providers included in the user flow.</span></span>|
|<span data-ttu-id="eab6a-169">userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="eab6a-169">userAttributeAssignments</span></span>|<span data-ttu-id="eab6a-170">Коллекция [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md)</span><span class="sxs-lookup"><span data-stu-id="eab6a-170">[identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) collection</span></span>|<span data-ttu-id="eab6a-171">Назначения атрибутов пользователя, включенные в поток пользователей.</span><span class="sxs-lookup"><span data-stu-id="eab6a-171">The user attribute assignments included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="eab6a-172">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eab6a-172">JSON representation</span></span>

<span data-ttu-id="eab6a-173">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eab6a-173">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.b2cIdentityUserFlow",
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
