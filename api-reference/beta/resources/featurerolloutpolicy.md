---
title: Тип ресурса featureRolloutPolicy
description: Представляет политику выката функций, связанную с объектом каталога.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: fa572cf9140a00d28b9db9d0e6a8e58fe6bb8969
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161672"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="bda04-103">Тип ресурса featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="bda04-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bda04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bda04-105">Представляет политику выката функций, связанную с объектом каталога.</span><span class="sxs-lookup"><span data-stu-id="bda04-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="bda04-106">Создание политики внедрения компонентов помогает администраторам клиентов пилотным функциям Azure AD с определенной группой перед включением функций для всей организации.</span><span class="sxs-lookup"><span data-stu-id="bda04-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="bda04-107">Это минимизирует влияние и помогает администраторам постепенно тестировать и тестировать связанные функции проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="bda04-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="bda04-108">Ниже данная возможность может быть ограниченной.</span><span class="sxs-lookup"><span data-stu-id="bda04-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="bda04-109">Каждая функция поддерживает не более 10 групп.</span><span class="sxs-lookup"><span data-stu-id="bda04-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="bda04-110">Поле **appliesTo** поддерживает только группы.</span><span class="sxs-lookup"><span data-stu-id="bda04-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="bda04-111">Динамические и вложенные группы не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="bda04-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="bda04-112">Ниже представлены предварительные требования для каждой функции, которая в настоящее время используется для применения этой политики.</span><span class="sxs-lookup"><span data-stu-id="bda04-112">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="bda04-113">Passthrough Authentication</span><span class="sxs-lookup"><span data-stu-id="bda04-113">Passthrough Authentication</span></span>

* <span data-ttu-id="bda04-114">Определите сервер под управлением Windows Server 2012 R2 или более поздней версии, на котором должен работать агент [PassthroughAuthentication.](/azure/active-directory/hybrid/how-to-connect-pta)</span><span class="sxs-lookup"><span data-stu-id="bda04-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="bda04-115">Убедитесь, что сервер присоединяется к домену, может проверить подлинность выбранных пользователей с помощью Active Directory и взаимодействовать с Azure AD через исходящие порты и URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="bda04-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="bda04-116">[Загрузите](https://aka.ms/getauthagent) & установить агент проверки подлинности Microsoft Azure AD Connect на сервере.</span><span class="sxs-lookup"><span data-stu-id="bda04-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="bda04-117">Чтобы обеспечить высокую доступность, установите дополнительные агенты проверки подлинности на другие серверы, как [описано здесь.](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)</span><span class="sxs-lookup"><span data-stu-id="bda04-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="bda04-118">Убедитесь, что вы правильно настроили параметры [интеллектуальной](/azure/active-directory/authentication/howto-password-smart-lockout) блокировки.</span><span class="sxs-lookup"><span data-stu-id="bda04-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="bda04-119">Это необходимо для того, чтобы учетные записи пользователей в локальной службе Active Directory не блокировали плохо активные субъекты.</span><span class="sxs-lookup"><span data-stu-id="bda04-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="bda04-120">SeamlessSso</span><span class="sxs-lookup"><span data-stu-id="bda04-120">SeamlessSso</span></span>

* <span data-ttu-id="bda04-121">В этом режиме в лесах AD в соответствии с этими [инструкциями](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) включается [seamlessSso.](/azure/active-directory/hybrid/how-to-connect-sso)</span><span class="sxs-lookup"><span data-stu-id="bda04-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="bda04-122">PasswordHashSync</span><span class="sxs-lookup"><span data-stu-id="bda04-122">PasswordHashSync</span></span>

* <span data-ttu-id="bda04-123">Включении [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs)со страницы "Необязательные   функции" в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="bda04-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

### <a name="emailasalternateid"></a><span data-ttu-id="bda04-124">EmailAsAlternateId</span><span class="sxs-lookup"><span data-stu-id="bda04-124">EmailAsAlternateId</span></span>

* <span data-ttu-id="bda04-125">Связывать альтернативную электронную почту с учетными записями пользователей.</span><span class="sxs-lookup"><span data-stu-id="bda04-125">Associate alternate email  with user accounts.</span></span>

## <a name="methods"></a><span data-ttu-id="bda04-126">Методы</span><span class="sxs-lookup"><span data-stu-id="bda04-126">Methods</span></span>

| <span data-ttu-id="bda04-127">Метод</span><span class="sxs-lookup"><span data-stu-id="bda04-127">Method</span></span>                                                                         | <span data-ttu-id="bda04-128">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="bda04-128">Return Type</span></span>                                     | <span data-ttu-id="bda04-129">Описание</span><span class="sxs-lookup"><span data-stu-id="bda04-129">Description</span></span>                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [<span data-ttu-id="bda04-130">Список featureRolloutPolicies</span><span class="sxs-lookup"><span data-stu-id="bda04-130">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="bda04-131">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="bda04-132">Получить список объектов featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="bda04-132">Retrieve a list of featureRolloutPolicy objects.</span></span>                          |
| [<span data-ttu-id="bda04-133">Get featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-133">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md)                 | [<span data-ttu-id="bda04-134">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="bda04-135">Извлечение свойств и связей объекта featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="bda04-135">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="bda04-136">Создание featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-136">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="bda04-137">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="bda04-138">Создание объекта featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="bda04-138">Create a new featureRolloutPolicy object.</span></span>                                 |
| [<span data-ttu-id="bda04-139">Обновление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md)           | [<span data-ttu-id="bda04-140">featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="bda04-141">Обновление свойств объекта featurerolloutpolicy.</span><span class="sxs-lookup"><span data-stu-id="bda04-141">Update the properties of featurerolloutpolicy object.</span></span>                     |
| [<span data-ttu-id="bda04-142">Удаление featureRolloutPolicy</span><span class="sxs-lookup"><span data-stu-id="bda04-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md)           | <span data-ttu-id="bda04-143">Нет</span><span class="sxs-lookup"><span data-stu-id="bda04-143">None</span></span>                                            | <span data-ttu-id="bda04-144">Удаление объекта featureRolloutPolicy.</span><span class="sxs-lookup"><span data-stu-id="bda04-144">Delete a featureRolloutPolicy object.</span></span>                                     |
| [<span data-ttu-id="bda04-145">Assign appliesTo</span><span class="sxs-lookup"><span data-stu-id="bda04-145">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md)              | [<span data-ttu-id="bda04-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="bda04-146">directoryObject</span></span>](directoryobject.md)           | <span data-ttu-id="bda04-147">Назначьте directoryObject для выдаваемой функции.</span><span class="sxs-lookup"><span data-stu-id="bda04-147">Assign a directoryObject to feature rollout.</span></span>                              |
| [<span data-ttu-id="bda04-148">Remove appliesTo</span><span class="sxs-lookup"><span data-stu-id="bda04-148">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md)            | <span data-ttu-id="bda04-149">Нет</span><span class="sxs-lookup"><span data-stu-id="bda04-149">None</span></span>                                            | <span data-ttu-id="bda04-150">Удаление directoryObject из проектов функций.</span><span class="sxs-lookup"><span data-stu-id="bda04-150">Remove a directoryObject from feature rollout.</span></span>                            |

## <a name="properties"></a><span data-ttu-id="bda04-151">Свойства</span><span class="sxs-lookup"><span data-stu-id="bda04-151">Properties</span></span>

| <span data-ttu-id="bda04-152">Свойство</span><span class="sxs-lookup"><span data-stu-id="bda04-152">Property</span></span>     | <span data-ttu-id="bda04-153">Тип</span><span class="sxs-lookup"><span data-stu-id="bda04-153">Type</span></span>        | <span data-ttu-id="bda04-154">Описание</span><span class="sxs-lookup"><span data-stu-id="bda04-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bda04-155">description</span><span class="sxs-lookup"><span data-stu-id="bda04-155">description</span></span>|<span data-ttu-id="bda04-156">String</span><span class="sxs-lookup"><span data-stu-id="bda04-156">String</span></span>|<span data-ttu-id="bda04-157">Описание этой политики выката функций.</span><span class="sxs-lookup"><span data-stu-id="bda04-157">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="bda04-158">displayName</span><span class="sxs-lookup"><span data-stu-id="bda04-158">displayName</span></span>|<span data-ttu-id="bda04-159">String</span><span class="sxs-lookup"><span data-stu-id="bda04-159">String</span></span>|<span data-ttu-id="bda04-160">Отображаемого имени для этой политики выката функций.</span><span class="sxs-lookup"><span data-stu-id="bda04-160">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="bda04-161">feature</span><span class="sxs-lookup"><span data-stu-id="bda04-161">feature</span></span>|<span data-ttu-id="bda04-162">stagedFeatureName</span><span class="sxs-lookup"><span data-stu-id="bda04-162">stagedFeatureName</span></span>| <span data-ttu-id="bda04-163">Возможные значения: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="bda04-163">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="bda04-164">id</span><span class="sxs-lookup"><span data-stu-id="bda04-164">id</span></span>|<span data-ttu-id="bda04-165">String</span><span class="sxs-lookup"><span data-stu-id="bda04-165">String</span></span>| <span data-ttu-id="bda04-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="bda04-166">Read-only.</span></span>|
|<span data-ttu-id="bda04-167">isAppliedToOrganization</span><span class="sxs-lookup"><span data-stu-id="bda04-167">isAppliedToOrganization</span></span>|<span data-ttu-id="bda04-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="bda04-168">Boolean</span></span>|<span data-ttu-id="bda04-169">Указывает, следует ли применять эту политику для всей организации.</span><span class="sxs-lookup"><span data-stu-id="bda04-169">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="bda04-170">isEnabled</span><span class="sxs-lookup"><span data-stu-id="bda04-170">isEnabled</span></span>|<span data-ttu-id="bda04-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="bda04-171">Boolean</span></span>|<span data-ttu-id="bda04-172">Указывает, включен ли выкат функции.</span><span class="sxs-lookup"><span data-stu-id="bda04-172">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bda04-173">Связи</span><span class="sxs-lookup"><span data-stu-id="bda04-173">Relationships</span></span>

| <span data-ttu-id="bda04-174">Связь</span><span class="sxs-lookup"><span data-stu-id="bda04-174">Relationship</span></span> | <span data-ttu-id="bda04-175">Тип</span><span class="sxs-lookup"><span data-stu-id="bda04-175">Type</span></span>        | <span data-ttu-id="bda04-176">Описание</span><span class="sxs-lookup"><span data-stu-id="bda04-176">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="bda04-177">appliesTo</span><span class="sxs-lookup"><span data-stu-id="bda04-177">appliesTo</span></span>|<span data-ttu-id="bda04-178">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="bda04-178">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="bda04-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="bda04-179">Nullable.</span></span> <span data-ttu-id="bda04-180">Указывает список directoryObjects, для которые включена функция.</span><span class="sxs-lookup"><span data-stu-id="bda04-180">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bda04-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bda04-181">JSON representation</span></span>

<span data-ttu-id="bda04-182">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="bda04-182">The following is a JSON representation of the resource.</span></span>

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


