---
title: тип ресурса featureRolloutPolicy
description: Представляет политику выкатки функций, связанную с объектом каталога.
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7fa35d99c8c77240a182b5d28a0fdb896153aa8b
ms.sourcegitcommit: 2006bf01c60793ac6ab1e25fa0526ec5d33c6334
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/23/2021
ms.locfileid: "51961137"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="17043-103">тип ресурса featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="17043-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="17043-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [feature-rolloutpolicy-deprecate](../../includes/directory-featurerolloutpolicies-deprecate.md)]

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17043-105">Представляет политику выкатки функций, связанную с объектом каталога.</span><span class="sxs-lookup"><span data-stu-id="17043-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="17043-106">Создание политики внедрения компонентов помогает администраторам клиентов пилотным функциям Azure AD с определенной группой, прежде чем включать функции для всей организации.</span><span class="sxs-lookup"><span data-stu-id="17043-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="17043-107">Это минимизирует влияние и помогает администраторам постепенно тестировать и выкатывать связанные функции проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="17043-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="17043-108">Ниже представлены ограничения для выкатки функций:</span><span class="sxs-lookup"><span data-stu-id="17043-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="17043-109">Каждая функция поддерживает не более 10 групп.</span><span class="sxs-lookup"><span data-stu-id="17043-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="17043-110">Поле **appliesTo** поддерживает только группы.</span><span class="sxs-lookup"><span data-stu-id="17043-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="17043-111">Динамические группы и вложенные группы не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="17043-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="17043-112">Ниже представлены предварительные требования к каждому из компонентов, которые в настоящее время поддерживаются для выкатки с помощью этой политики.</span><span class="sxs-lookup"><span data-stu-id="17043-112">The following are pre-requisites for each of the features that are currently supported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="17043-113">Проверка подлинности через проход</span><span class="sxs-lookup"><span data-stu-id="17043-113">Passthrough Authentication</span></span>

* <span data-ttu-id="17043-114">Определите сервер с Windows Server 2012 R2 или более поздней версии, на котором необходимо запустить агент [PassthroughAuthentication.](/azure/active-directory/hybrid/how-to-connect-pta)</span><span class="sxs-lookup"><span data-stu-id="17043-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="17043-115">Убедитесь, что сервер соединен с доменом, может проверить подлинность выбранных пользователей с помощью Active Directory и взаимодействовать с Azure AD в исходящие порты и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="17043-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="17043-116">[Скачайте](https://aka.ms/getauthagent) & установите агент проверки подлинности Microsoft Azure AD Connect на сервере.</span><span class="sxs-lookup"><span data-stu-id="17043-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="17043-117">Чтобы обеспечить высокую доступность, установите дополнительные агенты проверки подлинности на других серверах, как описано [здесь.](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)</span><span class="sxs-lookup"><span data-stu-id="17043-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="17043-118">Убедитесь, что вы правильно настроили параметры [smart lockout.](/azure/active-directory/authentication/howto-password-smart-lockout)</span><span class="sxs-lookup"><span data-stu-id="17043-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="17043-119">Это необходимо для обеспечения того, чтобы учетные записи активных каталогов пользователей не блокировалися плохими субъектами.</span><span class="sxs-lookup"><span data-stu-id="17043-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="17043-120">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="17043-120">SeamlessSso</span></span>

* <span data-ttu-id="17043-121">Включить [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) для лесов AD на основе [этих](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) инструкций.</span><span class="sxs-lookup"><span data-stu-id="17043-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="17043-122">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="17043-122">PasswordHashSync</span></span>

* <span data-ttu-id="17043-123">Включении [PasswordHashSync со](/azure/active-directory/hybrid/whatis-phs)   страницы "Необязательные функции" в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="17043-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

### <a name="emailasalternateid"></a><span data-ttu-id="17043-124">EmailAsAlternateId</span><span class="sxs-lookup"><span data-stu-id="17043-124">EmailAsAlternateId</span></span>

* <span data-ttu-id="17043-125">Связывать альтернативные сообщения электронной почты с учетными записями пользователей.</span><span class="sxs-lookup"><span data-stu-id="17043-125">Associate alternate email  with user accounts.</span></span>

## <a name="methods"></a><span data-ttu-id="17043-126">Методы</span><span class="sxs-lookup"><span data-stu-id="17043-126">Methods</span></span>

| <span data-ttu-id="17043-127">Метод</span><span class="sxs-lookup"><span data-stu-id="17043-127">Method</span></span>                                                                         | <span data-ttu-id="17043-128">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="17043-128">Return Type</span></span>                                     | <span data-ttu-id="17043-129">Описание</span><span class="sxs-lookup"><span data-stu-id="17043-129">Description</span></span>                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [<span data-ttu-id="17043-130">Функция ListRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="17043-130">List featureRolloutPolicies</span></span>](../api/list-featurerolloutpolicies.md) | [<span data-ttu-id="17043-131">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="17043-132">Извлечение списка объектов featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="17043-132">Retrieve a list of featureRolloutPolicy objects.</span></span>                          |
| [<span data-ttu-id="17043-133">Get featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-133">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md)                 | [<span data-ttu-id="17043-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="17043-135">Извлечение свойств и связей объекта featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="17043-135">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="17043-136">Создание featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-136">Create featureRolloutPolicy</span></span>](../api/post-featurerolloutpolicies.md) | [<span data-ttu-id="17043-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="17043-138">Создайте новый объект featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="17043-138">Create a new featureRolloutPolicy object.</span></span>                                 |
| [<span data-ttu-id="17043-139">Обновление функцииRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md)           | [<span data-ttu-id="17043-140">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="17043-141">Обновление свойств объекта featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="17043-141">Update the properties of featurerolloutpolicy object.</span></span>                     |
| [<span data-ttu-id="17043-142">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="17043-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md)           | <span data-ttu-id="17043-143">Нет</span><span class="sxs-lookup"><span data-stu-id="17043-143">None</span></span>                                            | <span data-ttu-id="17043-144">Удаление объекта featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="17043-144">Delete a featureRolloutPolicy object.</span></span>                                     |
| [<span data-ttu-id="17043-145">Назначение appliesTo</span><span class="sxs-lookup"><span data-stu-id="17043-145">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md)              | [<span data-ttu-id="17043-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="17043-146">directoryObject</span></span>](directoryobject.md)           | <span data-ttu-id="17043-147">Назначение каталогаОбект для выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="17043-147">Assign a directoryObject to feature rollout.</span></span>                              |
| [<span data-ttu-id="17043-148">Удаление appliesTo</span><span class="sxs-lookup"><span data-stu-id="17043-148">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md)            | <span data-ttu-id="17043-149">Нет</span><span class="sxs-lookup"><span data-stu-id="17043-149">None</span></span>                                            | <span data-ttu-id="17043-150">Удалите directoryObject из выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="17043-150">Remove a directoryObject from feature rollout.</span></span>                            |

## <a name="properties"></a><span data-ttu-id="17043-151">Свойства</span><span class="sxs-lookup"><span data-stu-id="17043-151">Properties</span></span>

| <span data-ttu-id="17043-152">Свойство</span><span class="sxs-lookup"><span data-stu-id="17043-152">Property</span></span>     | <span data-ttu-id="17043-153">Тип</span><span class="sxs-lookup"><span data-stu-id="17043-153">Type</span></span>        | <span data-ttu-id="17043-154">Описание</span><span class="sxs-lookup"><span data-stu-id="17043-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17043-155">description</span><span class="sxs-lookup"><span data-stu-id="17043-155">description</span></span>|<span data-ttu-id="17043-156">String</span><span class="sxs-lookup"><span data-stu-id="17043-156">String</span></span>|<span data-ttu-id="17043-157">Описание этой политики выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="17043-157">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="17043-158">displayName</span><span class="sxs-lookup"><span data-stu-id="17043-158">displayName</span></span>|<span data-ttu-id="17043-159">String</span><span class="sxs-lookup"><span data-stu-id="17043-159">String</span></span>|<span data-ttu-id="17043-160">Имя отображения для этой политики выкатки функций.</span><span class="sxs-lookup"><span data-stu-id="17043-160">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="17043-161">функция</span><span class="sxs-lookup"><span data-stu-id="17043-161">feature</span></span>|<span data-ttu-id="17043-162">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="17043-162">stagedFeatureName</span></span>| <span data-ttu-id="17043-163">Возможные значения: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `emailAsAlternateId`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="17043-163">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `emailAsAlternateId`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="17043-164">id</span><span class="sxs-lookup"><span data-stu-id="17043-164">id</span></span>|<span data-ttu-id="17043-165">String</span><span class="sxs-lookup"><span data-stu-id="17043-165">String</span></span>| <span data-ttu-id="17043-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="17043-166">Read-only.</span></span>|
|<span data-ttu-id="17043-167">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="17043-167">isAppliedToOrganization</span></span>|<span data-ttu-id="17043-168">Логический</span><span class="sxs-lookup"><span data-stu-id="17043-168">Boolean</span></span>|<span data-ttu-id="17043-169">Указывает, следует ли применять эту политику выкатки функций ко всей организации.</span><span class="sxs-lookup"><span data-stu-id="17043-169">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="17043-170">isEnabled</span><span class="sxs-lookup"><span data-stu-id="17043-170">isEnabled</span></span>|<span data-ttu-id="17043-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="17043-171">Boolean</span></span>|<span data-ttu-id="17043-172">Указывает, включена ли выкатка функций.</span><span class="sxs-lookup"><span data-stu-id="17043-172">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="17043-173">Связи</span><span class="sxs-lookup"><span data-stu-id="17043-173">Relationships</span></span>

| <span data-ttu-id="17043-174">Связь</span><span class="sxs-lookup"><span data-stu-id="17043-174">Relationship</span></span> | <span data-ttu-id="17043-175">Тип</span><span class="sxs-lookup"><span data-stu-id="17043-175">Type</span></span>        | <span data-ttu-id="17043-176">Описание</span><span class="sxs-lookup"><span data-stu-id="17043-176">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="17043-177">appliesTo</span><span class="sxs-lookup"><span data-stu-id="17043-177">appliesTo</span></span>|<span data-ttu-id="17043-178">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="17043-178">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="17043-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="17043-179">Nullable.</span></span> <span data-ttu-id="17043-180">Указывает список directoryObjects, для которые включена функция.</span><span class="sxs-lookup"><span data-stu-id="17043-180">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="17043-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="17043-181">JSON representation</span></span>

<span data-ttu-id="17043-182">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="17043-182">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


