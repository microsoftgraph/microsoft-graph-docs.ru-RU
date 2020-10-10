---
title: Тип ресурса b2cIdentityUserFlow
description: Представляет пользовательский поток в клиенте Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: af29926d77c8888cadc67c4cd7e7558fe47062d6
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406486"
---
# <a name="b2cidentityuserflow-resource-type"></a><span data-ttu-id="3c692-103">Тип ресурса b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3c692-103">b2cIdentityUserFlow resource type</span></span>

<span data-ttu-id="3c692-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c692-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c692-105">Представляет пользовательский поток в клиенте Azure Active Directory B2C.</span><span class="sxs-lookup"><span data-stu-id="3c692-105">Represents a user flow within an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="3c692-106">Чтобы помочь с настройкой наиболее распространенных задач идентификации для ваших приложений, Azure Active Directory B2C содержит заранее определенные настраиваемые политики, называемые [пользовательскими потоками](/azure/active-directory-b2c/user-flow-overview).</span><span class="sxs-lookup"><span data-stu-id="3c692-106">To help you set up the most common identity tasks for your applications, Azure Active Directory B2C includes predefined, configurable policies called [user flows](/azure/active-directory-b2c/user-flow-overview).</span></span> <span data-ttu-id="3c692-107">Пользовательский поток позволяет вам определить, как пользователи взаимодействуют с вашим приложением, когда они выполняют такие задачи, как вход, регистрация, изменение профиля или сброс пароля.</span><span class="sxs-lookup"><span data-stu-id="3c692-107">A user flow lets you determine how users interact with your application when they do things like sign in, sign up, edit a profile, or reset a password.</span></span> <span data-ttu-id="3c692-108">Вы можете создать множество пользовательских потоков различных типов в своем клиенте и использовать их в приложении по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="3c692-108">You can create many user flows of different types in your tenant and use them in your applications as needed.</span></span> <span data-ttu-id="3c692-109">С помощью пользовательских потоков вы можете управлять следующими возможностями:</span><span class="sxs-lookup"><span data-stu-id="3c692-109">With user flows, you can control the following capabilities:</span></span>

- <span data-ttu-id="3c692-110">Типы учетных записей, используемые для входа, например учетные записи социальных сетей, таких как Facebook, или локальные учетные записи</span><span class="sxs-lookup"><span data-stu-id="3c692-110">Account types used for sign-in, such as social accounts like a Facebook or local account</span></span>
- <span data-ttu-id="3c692-111">Атрибуты, собираемые у пользователей, такие как имя, почтовый индекс и размер обуви</span><span class="sxs-lookup"><span data-stu-id="3c692-111">Attributes to be collected from the consumer, such as first name, postal code, and shoe size</span></span>
- <span data-ttu-id="3c692-112">Многофакторная проверка подлинности Azure</span><span class="sxs-lookup"><span data-stu-id="3c692-112">Azure Multi-Factor Authentication</span></span>
- <span data-ttu-id="3c692-113">Настройка пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="3c692-113">Customization of the user interface</span></span>
- <span data-ttu-id="3c692-114">Сведения, получаемые приложением в маркере</span><span class="sxs-lookup"><span data-stu-id="3c692-114">Information that the application receives in the token</span></span>

## <a name="methods"></a><span data-ttu-id="3c692-115">Методы</span><span class="sxs-lookup"><span data-stu-id="3c692-115">Methods</span></span>

| <span data-ttu-id="3c692-116">Метод</span><span class="sxs-lookup"><span data-stu-id="3c692-116">Method</span></span>       | <span data-ttu-id="3c692-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="3c692-117">Return Type</span></span>  |<span data-ttu-id="3c692-118">Описание</span><span class="sxs-lookup"><span data-stu-id="3c692-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="3c692-119">Перечисление пользовательских потоков</span><span class="sxs-lookup"><span data-stu-id="3c692-119">List user flows</span></span>](../api/identitycontainer-list-b2cuserflows.md)|<span data-ttu-id="3c692-120">Коллекция b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3c692-120">b2cIdentityUserFlow collection</span></span>|<span data-ttu-id="3c692-121">Извлечение всех пользовательских потоков B2C.</span><span class="sxs-lookup"><span data-stu-id="3c692-121">Retrieve all B2C user flows.</span></span>|
|[<span data-ttu-id="3c692-122">Получение пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="3c692-122">Get user flow</span></span>](../api/b2cidentityuserflow-get.md)|<span data-ttu-id="3c692-123">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3c692-123">b2cIdentityUserFlow</span></span>|<span data-ttu-id="3c692-124">Извлечение свойств пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="3c692-124">Retrieve properties of a B2C user flow.</span></span>|
|[<span data-ttu-id="3c692-125">Создание пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="3c692-125">Create user flow</span></span>](../api/identitycontainer-post-b2cuserflows.md)|<span data-ttu-id="3c692-126">b2cIdentityUserFlow</span><span class="sxs-lookup"><span data-stu-id="3c692-126">b2cIdentityUserFlow</span></span>|<span data-ttu-id="3c692-127">Создание пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="3c692-127">Create a new B2C user flow.</span></span>|
|[<span data-ttu-id="3c692-128">Удаление пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="3c692-128">Delete user flow</span></span>](../api/b2cidentityuserflow-delete.md)|<span data-ttu-id="3c692-129">Нет</span><span class="sxs-lookup"><span data-stu-id="3c692-129">None</span></span>|<span data-ttu-id="3c692-130">Удаление пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="3c692-130">Delete a B2C user flow.</span></span>|
|[<span data-ttu-id="3c692-131">Перечисление поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="3c692-131">List identity providers</span></span>](../api/b2cidentityuserflow-list-identityproviders.md)|<span data-ttu-id="3c692-132">Коллекция объектов [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="3c692-132">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="3c692-133">Получение всех поставщиков удостоверений в пользовательском потоке B2C.</span><span class="sxs-lookup"><span data-stu-id="3c692-133">Retrieve all identity providers in a B2C user flow.</span></span>|
|[<span data-ttu-id="3c692-134">Добавление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="3c692-134">Add identity provider</span></span>](../api/b2cidentityuserflow-post-identityproviders.md)|<span data-ttu-id="3c692-135">Нет</span><span class="sxs-lookup"><span data-stu-id="3c692-135">None</span></span>|<span data-ttu-id="3c692-136">Добавление поставщика удостоверений в пользовательский поток B2C.</span><span class="sxs-lookup"><span data-stu-id="3c692-136">Add an identity provider to a B2C user flow.</span></span>|
|[<span data-ttu-id="3c692-137">Удаление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="3c692-137">Remove identity provider</span></span>](../api/b2cidentityuserflow-delete-identityproviders.md)|<span data-ttu-id="3c692-138">Нет</span><span class="sxs-lookup"><span data-stu-id="3c692-138">None</span></span>|<span data-ttu-id="3c692-139">Удаление поставщика удостоверений из пользовательского потока B2C.</span><span class="sxs-lookup"><span data-stu-id="3c692-139">Remove an identity provider from a B2C user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="3c692-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="3c692-140">Properties</span></span>

|<span data-ttu-id="3c692-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="3c692-141">Property</span></span>|<span data-ttu-id="3c692-142">Тип</span><span class="sxs-lookup"><span data-stu-id="3c692-142">Type</span></span>|<span data-ttu-id="3c692-143">Описание</span><span class="sxs-lookup"><span data-stu-id="3c692-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c692-144">id</span><span class="sxs-lookup"><span data-stu-id="3c692-144">id</span></span>|<span data-ttu-id="3c692-145">Строка</span><span class="sxs-lookup"><span data-stu-id="3c692-145">String</span></span>|<span data-ttu-id="3c692-146">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="3c692-146">The name of the user flow.</span></span> <span data-ttu-id="3c692-147">Это обязательное значение, не изменяемое после создания.</span><span class="sxs-lookup"><span data-stu-id="3c692-147">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="3c692-148">После создания перед именем будет добавлен префикс со значением `B2C_1_`.</span><span class="sxs-lookup"><span data-stu-id="3c692-148">The name will be prefixed with the value of `B2C_1_` after creation.</span></span>|
|<span data-ttu-id="3c692-149">userFlowType</span><span class="sxs-lookup"><span data-stu-id="3c692-149">userFlowType</span></span>|<span data-ttu-id="3c692-150">Строка</span><span class="sxs-lookup"><span data-stu-id="3c692-150">String</span></span>|<span data-ttu-id="3c692-151">[Тип пользовательского потока](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span><span class="sxs-lookup"><span data-stu-id="3c692-151">The [type of user flow](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span></span> <span data-ttu-id="3c692-152">Поддерживаемые значения для **userFlowType**:</span><span class="sxs-lookup"><span data-stu-id="3c692-152">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="3c692-153">userFlowTypeVersion</span><span class="sxs-lookup"><span data-stu-id="3c692-153">userFlowTypeVersion</span></span>|<span data-ttu-id="3c692-154">Одинарное</span><span class="sxs-lookup"><span data-stu-id="3c692-154">Single</span></span>|<span data-ttu-id="3c692-155">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="3c692-155">The version of the user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c692-156">Связи</span><span class="sxs-lookup"><span data-stu-id="3c692-156">Relationships</span></span>

| <span data-ttu-id="3c692-157">Связь</span><span class="sxs-lookup"><span data-stu-id="3c692-157">Relationship</span></span>       | <span data-ttu-id="3c692-158">Тип</span><span class="sxs-lookup"><span data-stu-id="3c692-158">Type</span></span>  |<span data-ttu-id="3c692-159">Описание</span><span class="sxs-lookup"><span data-stu-id="3c692-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c692-160">identityProviders</span><span class="sxs-lookup"><span data-stu-id="3c692-160">identityProviders</span></span>|<span data-ttu-id="3c692-161">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="3c692-161">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="3c692-162">Поставщики удостоверений, включенные в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="3c692-162">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c692-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3c692-163">JSON representation</span></span>

<span data-ttu-id="3c692-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3c692-164">The following is a JSON representation of the resource.</span></span>

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
    "identityProviders": [{"@odata.type": "microsoft.graph.identityProvider"}]
}
```