---
title: Тип ресурса b2cUserFlows
description: Представляет пользовательский поток в клиенте Azure Active Directory B2C.
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: 68df559afb6937befeab27c129d951a4c1e7ad20
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089778"
---
# <a name="b2cuserflows-resource-type"></a><span data-ttu-id="38a64-103">Тип ресурса b2cUserFlows</span><span class="sxs-lookup"><span data-stu-id="38a64-103">b2cUserFlows resource type</span></span>

<span data-ttu-id="38a64-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="38a64-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38a64-105">Представляет пользовательский поток в клиенте Azure Active Directory B2C.</span><span class="sxs-lookup"><span data-stu-id="38a64-105">Represents a user flow within an Azure Active Directory B2C tenant.</span></span>

<span data-ttu-id="38a64-106">Чтобы помочь с настройкой наиболее распространенных задач идентификации для ваших приложений, Azure Active Directory B2C содержит заранее определенные настраиваемые политики, называемые [пользовательскими потоками](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-overview).</span><span class="sxs-lookup"><span data-stu-id="38a64-106">To help you set up the most common identity tasks for your applications, Azure Active Directory B2C includes predefined, configurable policies called [user flows](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-overview).</span></span> <span data-ttu-id="38a64-107">Пользовательский поток позволяет вам определить, как пользователи взаимодействуют с вашим приложением, когда они выполняют такие задачи, как вход, регистрация, изменение профиля или сброс пароля.</span><span class="sxs-lookup"><span data-stu-id="38a64-107">A user flow lets you determine how users interact with your application when they do things like sign in, sign up, edit a profile, or reset a password.</span></span> <span data-ttu-id="38a64-108">Вы можете создать множество пользовательских потоков различных типов в своем клиенте и использовать их в приложении по мере необходимости.</span><span class="sxs-lookup"><span data-stu-id="38a64-108">You can create many user flows of different types in your tenant and use them in your applications as needed.</span></span> <span data-ttu-id="38a64-109">С помощью пользовательских потоков вы можете управлять следующими возможностями:</span><span class="sxs-lookup"><span data-stu-id="38a64-109">With user flows, you can control the following capabilities:</span></span>

- <span data-ttu-id="38a64-110">Типы учетных записей, используемые для входа, например учетные записи социальных сетей, таких как Facebook, или локальные учетные записи</span><span class="sxs-lookup"><span data-stu-id="38a64-110">Account types used for sign-in, such as social accounts like a Facebook or local account</span></span>
- <span data-ttu-id="38a64-111">Атрибуты, собираемые у пользователей, такие как имя, почтовый индекс и размер обуви</span><span class="sxs-lookup"><span data-stu-id="38a64-111">Attributes to be collected from the consumer, such as first name, postal code, and shoe size</span></span>
- <span data-ttu-id="38a64-112">Многофакторная проверка подлинности Azure</span><span class="sxs-lookup"><span data-stu-id="38a64-112">Azure Multi-Factor Authentication</span></span>
- <span data-ttu-id="38a64-113">Настройка пользовательского интерфейса</span><span class="sxs-lookup"><span data-stu-id="38a64-113">Customization of the user interface</span></span>
- <span data-ttu-id="38a64-114">Сведения, получаемые приложением в маркере</span><span class="sxs-lookup"><span data-stu-id="38a64-114">Information that the application receives in the token</span></span>

## <a name="methods"></a><span data-ttu-id="38a64-115">Методы</span><span class="sxs-lookup"><span data-stu-id="38a64-115">Methods</span></span>

| <span data-ttu-id="38a64-116">Метод</span><span class="sxs-lookup"><span data-stu-id="38a64-116">Method</span></span>       | <span data-ttu-id="38a64-117">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="38a64-117">Return Type</span></span>  |<span data-ttu-id="38a64-118">Описание</span><span class="sxs-lookup"><span data-stu-id="38a64-118">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="38a64-119">Перечисление пользовательских потоков</span><span class="sxs-lookup"><span data-stu-id="38a64-119">List user flows</span></span>](../api/b2cuserflows-list.md)|<span data-ttu-id="38a64-120">Коллекция b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="38a64-120">b2cUserFlow collection</span></span>|<span data-ttu-id="38a64-121">Извлечение всех пользовательских потоков.</span><span class="sxs-lookup"><span data-stu-id="38a64-121">Retrieve all user flows.</span></span>|
|[<span data-ttu-id="38a64-122">Получение пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="38a64-122">Get user flow</span></span>](../api/b2cuserflows-get.md)|<span data-ttu-id="38a64-123">b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="38a64-123">b2cUserFlow</span></span>|<span data-ttu-id="38a64-124">Извлечение свойств пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="38a64-124">Retrieve properties of a user flow.</span></span>|
|[<span data-ttu-id="38a64-125">Создание пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="38a64-125">Create user flow</span></span>](../api/b2cuserflow-post-b2cuserflows.md)|<span data-ttu-id="38a64-126">b2cUserFlow</span><span class="sxs-lookup"><span data-stu-id="38a64-126">b2cUserFlow</span></span>|<span data-ttu-id="38a64-127">Создание пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="38a64-127">Create a new user flow.</span></span>|
|[<span data-ttu-id="38a64-128">Удаление пользовательского потока</span><span class="sxs-lookup"><span data-stu-id="38a64-128">Delete user flow</span></span>](../api/b2cuserflows-delete.md)|<span data-ttu-id="38a64-129">Нет</span><span class="sxs-lookup"><span data-stu-id="38a64-129">None</span></span>|<span data-ttu-id="38a64-130">Удаление пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="38a64-130">Delete a user flow.</span></span>|
|[<span data-ttu-id="38a64-131">Перечисление поставщиков удостоверений</span><span class="sxs-lookup"><span data-stu-id="38a64-131">List identity providers</span></span>](../api/b2cuserflows-list-identityproviders.md)|<span data-ttu-id="38a64-132">Коллекция объектов [identityProvider](../resources/identityProvider.md)</span><span class="sxs-lookup"><span data-stu-id="38a64-132">[identityProvider](../resources/identityProvider.md) collection</span></span>|<span data-ttu-id="38a64-133">Получение всех поставщиков удостоверений в пользовательском потоке.</span><span class="sxs-lookup"><span data-stu-id="38a64-133">Retrieve all identity providers in a user flow.</span></span>|
|[<span data-ttu-id="38a64-134">Добавление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="38a64-134">Add identity provider</span></span>](../api/b2cuserflows-update-identityprovider.md)|<span data-ttu-id="38a64-135">Нет</span><span class="sxs-lookup"><span data-stu-id="38a64-135">None</span></span>|<span data-ttu-id="38a64-136">Добавление поставщика удостоверений в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="38a64-136">Add an identity provider to a user flow.</span></span>|
|[<span data-ttu-id="38a64-137">Удаление поставщика удостоверений</span><span class="sxs-lookup"><span data-stu-id="38a64-137">Delete identity provider</span></span>](../api/b2cuserflows-delete-identityprovider.md)|<span data-ttu-id="38a64-138">Нет</span><span class="sxs-lookup"><span data-stu-id="38a64-138">None</span></span>|<span data-ttu-id="38a64-139">Удаление поставщика удостоверений из пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="38a64-139">Delete an identity provider from a user flow.</span></span>|

## <a name="properties"></a><span data-ttu-id="38a64-140">Свойства</span><span class="sxs-lookup"><span data-stu-id="38a64-140">Properties</span></span>

|<span data-ttu-id="38a64-141">Свойство</span><span class="sxs-lookup"><span data-stu-id="38a64-141">Property</span></span>|<span data-ttu-id="38a64-142">Тип</span><span class="sxs-lookup"><span data-stu-id="38a64-142">Type</span></span>|<span data-ttu-id="38a64-143">Описание</span><span class="sxs-lookup"><span data-stu-id="38a64-143">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38a64-144">id</span><span class="sxs-lookup"><span data-stu-id="38a64-144">id</span></span>|<span data-ttu-id="38a64-145">Строка</span><span class="sxs-lookup"><span data-stu-id="38a64-145">String</span></span>|<span data-ttu-id="38a64-146">Имя пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="38a64-146">The name of the user flow.</span></span> <span data-ttu-id="38a64-147">Это обязательное значение, не изменяемое после создания.</span><span class="sxs-lookup"><span data-stu-id="38a64-147">This is a required value and is immutable after it's created.</span></span> <span data-ttu-id="38a64-148">После создания перед именем будет добавлен префикс со значением `B2C_1_`.</span><span class="sxs-lookup"><span data-stu-id="38a64-148">The name will be prefixed with the value of `B2C_1_` after creation.</span></span>|
|<span data-ttu-id="38a64-149">userFlowType</span><span class="sxs-lookup"><span data-stu-id="38a64-149">userFlowType</span></span>|<span data-ttu-id="38a64-150">Строка</span><span class="sxs-lookup"><span data-stu-id="38a64-150">String</span></span>|<span data-ttu-id="38a64-151">[Тип пользовательского потока](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span><span class="sxs-lookup"><span data-stu-id="38a64-151">The [type of user flow](https://docs.microsoft.com/azure/active-directory-b2c/user-flow-versions).</span></span> <span data-ttu-id="38a64-152">Поддерживаемые значения для **userFlowType**:</span><span class="sxs-lookup"><span data-stu-id="38a64-152">The supported values for **userFlowType** are:</span></span><br/><ul><li>`signUp`</li><li>`signIn`</li><li>`signUpOrSignIn`</li><li>`passwordReset`</li><li>`profileUpdate`</li><li>`resourceOwnerPasswordCredentialSignIn`</li>|
|<span data-ttu-id="38a64-153">userFlowVersion</span><span class="sxs-lookup"><span data-stu-id="38a64-153">userFlowVersion</span></span>|<span data-ttu-id="38a64-154">Одинарное</span><span class="sxs-lookup"><span data-stu-id="38a64-154">Single</span></span>|<span data-ttu-id="38a64-155">Версия пользовательского потока.</span><span class="sxs-lookup"><span data-stu-id="38a64-155">The version of the user flow.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38a64-156">Связи</span><span class="sxs-lookup"><span data-stu-id="38a64-156">Relationships</span></span>

| <span data-ttu-id="38a64-157">Связь</span><span class="sxs-lookup"><span data-stu-id="38a64-157">Relationship</span></span>       | <span data-ttu-id="38a64-158">Тип</span><span class="sxs-lookup"><span data-stu-id="38a64-158">Type</span></span>  |<span data-ttu-id="38a64-159">Описание</span><span class="sxs-lookup"><span data-stu-id="38a64-159">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38a64-160">identityProviders</span><span class="sxs-lookup"><span data-stu-id="38a64-160">identityProviders</span></span>|<span data-ttu-id="38a64-161">Коллекция объектов [identityProvider](../resources/identityprovider.md)</span><span class="sxs-lookup"><span data-stu-id="38a64-161">[identityProvider](../resources/identityprovider.md) collection</span></span>|<span data-ttu-id="38a64-162">Поставщики удостоверений, включенные в пользовательский поток.</span><span class="sxs-lookup"><span data-stu-id="38a64-162">The identity providers included in the user flow.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="38a64-163">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="38a64-163">JSON representation</span></span>

<span data-ttu-id="38a64-164">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="38a64-164">The following is a JSON representation of the resource.</span></span>

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


