---
title: Тип ресурса Феатурероллаутполици
description: Представляет политику развертывания компонентов, связанную с объектом каталога.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5c514d6a48ffafc13a118b9471fb94be9ffc0e11
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48071217"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="8c96f-103">Тип ресурса Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="8c96f-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c96f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c96f-105">Представляет политику развертывания компонентов, связанную с объектом каталога.</span><span class="sxs-lookup"><span data-stu-id="8c96f-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="8c96f-106">Создание политики развертывания компонентов поможет администраторам клиентов пилотно использовать определенную группу перед включением функций для всей Организации.</span><span class="sxs-lookup"><span data-stu-id="8c96f-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="8c96f-107">Это минимизирует воздействие и помогает администраторам постепенно тестировать и отменять связанные функции проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8c96f-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="8c96f-108">Ниже приведены ограничения на развертывание функций.</span><span class="sxs-lookup"><span data-stu-id="8c96f-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="8c96f-109">Каждая функция поддерживает не более 10 групп.</span><span class="sxs-lookup"><span data-stu-id="8c96f-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="8c96f-110">Поле **appliesTo** поддерживает только группы.</span><span class="sxs-lookup"><span data-stu-id="8c96f-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="8c96f-111">Динамические группы и вложенные группы не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="8c96f-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="8c96f-112">Ниже приведены предварительные требования для каждой из функций, которые в настоящее время супортед для развертывания с помощью этой политики развертывания.</span><span class="sxs-lookup"><span data-stu-id="8c96f-112">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="8c96f-113">Сквозная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="8c96f-113">Passthrough Authentication</span></span>

* <span data-ttu-id="8c96f-114">Определите сервер под управлением Windows Server 2012 R2 или более поздней версии, на котором нужно запустить агент [пасссраугхаусентикатион](/azure/active-directory/hybrid/how-to-connect-pta) .</span><span class="sxs-lookup"><span data-stu-id="8c96f-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="8c96f-115">Убедитесь, что сервер присоединен к домену, может выполнять проверку подлинности выбранных пользователей с помощью Active Directory и может связываться с Azure AD на исходящих портах/URL-адресах.</span><span class="sxs-lookup"><span data-stu-id="8c96f-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="8c96f-116">[Скачайте](https://aka.ms/getauthagent) & установить агент проверки подлинности Microsoft Azure AD Connect на сервере.</span><span class="sxs-lookup"><span data-stu-id="8c96f-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="8c96f-117">Чтобы обеспечить высокий уровень доступности, установите дополнительные агенты проверки подлинности на других серверах, как описано [здесь](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span><span class="sxs-lookup"><span data-stu-id="8c96f-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="8c96f-118">Убедитесь, что параметры [интеллектуальной блокировки](/azure/active-directory/authentication/howto-password-smart-lockout) настроены соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="8c96f-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="8c96f-119">Это необходимо для того, чтобы локальные учетные записи пользователей Active Directory не блокировались с помощью недопустимых субъектов.</span><span class="sxs-lookup"><span data-stu-id="8c96f-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="8c96f-120">сеамлессссо</span><span class="sxs-lookup"><span data-stu-id="8c96f-120">SeamlessSso</span></span>

* <span data-ttu-id="8c96f-121">Включите [сеамлессссо](/azure/active-directory/hybrid/how-to-connect-sso) для лесов Active Directory в соответствии с [этими](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) инструкциями.</span><span class="sxs-lookup"><span data-stu-id="8c96f-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="8c96f-122">пассвордхашсинк</span><span class="sxs-lookup"><span data-stu-id="8c96f-122">PasswordHashSync</span></span>

* <span data-ttu-id="8c96f-123">Включите [пассвордхашсинк](/azure/active-directory/hybrid/whatis-phs)   на странице "дополнительные компоненты" в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="8c96f-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

### <a name="emailasalternateid"></a><span data-ttu-id="8c96f-124">емаиласалтернатеид</span><span class="sxs-lookup"><span data-stu-id="8c96f-124">EmailAsAlternateId</span></span>

* <span data-ttu-id="8c96f-125">Свяжите альтернативную электронную почту с учетными записями пользователей.</span><span class="sxs-lookup"><span data-stu-id="8c96f-125">Associate alternate email  with user accounts.</span></span>

## <a name="methods"></a><span data-ttu-id="8c96f-126">Методы</span><span class="sxs-lookup"><span data-stu-id="8c96f-126">Methods</span></span>

| <span data-ttu-id="8c96f-127">Метод</span><span class="sxs-lookup"><span data-stu-id="8c96f-127">Method</span></span>                                                                         | <span data-ttu-id="8c96f-128">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="8c96f-128">Return Type</span></span>                                     | <span data-ttu-id="8c96f-129">Описание</span><span class="sxs-lookup"><span data-stu-id="8c96f-129">Description</span></span>                                                               |
|:-------------------------------------------------------------------------------|:------------------------------------------------|:--------------------------------------------------------------------------|
| [<span data-ttu-id="8c96f-130">Список ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="8c96f-130">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="8c96f-131">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="8c96f-132">Получение списка объектов Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="8c96f-132">Retrieve a list of featureRolloutPolicy objects.</span></span>                          |
| [<span data-ttu-id="8c96f-133">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-133">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md)                 | [<span data-ttu-id="8c96f-134">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="8c96f-135">Получение свойств и связей объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="8c96f-135">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="8c96f-136">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-136">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="8c96f-137">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="8c96f-138">Создание нового объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="8c96f-138">Create a new featureRolloutPolicy object.</span></span>                                 |
| [<span data-ttu-id="8c96f-139">Обновление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-139">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md)           | [<span data-ttu-id="8c96f-140">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-140">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="8c96f-141">Обновление свойств объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="8c96f-141">Update the properties of featurerolloutpolicy object.</span></span>                     |
| [<span data-ttu-id="8c96f-142">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="8c96f-142">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md)           | <span data-ttu-id="8c96f-143">Нет</span><span class="sxs-lookup"><span data-stu-id="8c96f-143">None</span></span>                                            | <span data-ttu-id="8c96f-144">Удаление объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="8c96f-144">Delete a featureRolloutPolicy object.</span></span>                                     |
| [<span data-ttu-id="8c96f-145">Назначение appliesTo</span><span class="sxs-lookup"><span data-stu-id="8c96f-145">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md)              | [<span data-ttu-id="8c96f-146">directoryObject</span><span class="sxs-lookup"><span data-stu-id="8c96f-146">directoryObject</span></span>](directoryobject.md)           | <span data-ttu-id="8c96f-147">Назначение directoryObject для развертывания компонентов.</span><span class="sxs-lookup"><span data-stu-id="8c96f-147">Assign a directoryObject to feature rollout.</span></span>                              |
| [<span data-ttu-id="8c96f-148">Удаление appliesTo</span><span class="sxs-lookup"><span data-stu-id="8c96f-148">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md)            | <span data-ttu-id="8c96f-149">Нет</span><span class="sxs-lookup"><span data-stu-id="8c96f-149">None</span></span>                                            | <span data-ttu-id="8c96f-150">Удаление directoryObject из развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="8c96f-150">Remove a directoryObject from feature rollout.</span></span>                            |

## <a name="properties"></a><span data-ttu-id="8c96f-151">Свойства</span><span class="sxs-lookup"><span data-stu-id="8c96f-151">Properties</span></span>

| <span data-ttu-id="8c96f-152">Свойство</span><span class="sxs-lookup"><span data-stu-id="8c96f-152">Property</span></span>     | <span data-ttu-id="8c96f-153">Тип</span><span class="sxs-lookup"><span data-stu-id="8c96f-153">Type</span></span>        | <span data-ttu-id="8c96f-154">Описание</span><span class="sxs-lookup"><span data-stu-id="8c96f-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c96f-155">description</span><span class="sxs-lookup"><span data-stu-id="8c96f-155">description</span></span>|<span data-ttu-id="8c96f-156">String</span><span class="sxs-lookup"><span data-stu-id="8c96f-156">String</span></span>|<span data-ttu-id="8c96f-157">Описание этой политики развертывания функций.</span><span class="sxs-lookup"><span data-stu-id="8c96f-157">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="8c96f-158">displayName</span><span class="sxs-lookup"><span data-stu-id="8c96f-158">displayName</span></span>|<span data-ttu-id="8c96f-159">String</span><span class="sxs-lookup"><span data-stu-id="8c96f-159">String</span></span>|<span data-ttu-id="8c96f-160">Отображаемое имя для этой политики развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="8c96f-160">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="8c96f-161">состав</span><span class="sxs-lookup"><span data-stu-id="8c96f-161">feature</span></span>|<span data-ttu-id="8c96f-162">стажедфеатуренаме</span><span class="sxs-lookup"><span data-stu-id="8c96f-162">stagedFeatureName</span></span>| <span data-ttu-id="8c96f-163">Возможные значения: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="8c96f-163">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8c96f-164">id</span><span class="sxs-lookup"><span data-stu-id="8c96f-164">id</span></span>|<span data-ttu-id="8c96f-165">String</span><span class="sxs-lookup"><span data-stu-id="8c96f-165">String</span></span>| <span data-ttu-id="8c96f-166">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="8c96f-166">Read-only.</span></span>|
|<span data-ttu-id="8c96f-167">исапплиедтурганизатион</span><span class="sxs-lookup"><span data-stu-id="8c96f-167">isAppliedToOrganization</span></span>|<span data-ttu-id="8c96f-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c96f-168">Boolean</span></span>|<span data-ttu-id="8c96f-169">Указывает, следует ли применять эту политику развертывания функций ко всей Организации.</span><span class="sxs-lookup"><span data-stu-id="8c96f-169">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="8c96f-170">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8c96f-170">isEnabled</span></span>|<span data-ttu-id="8c96f-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c96f-171">Boolean</span></span>|<span data-ttu-id="8c96f-172">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="8c96f-172">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c96f-173">Отношения</span><span class="sxs-lookup"><span data-stu-id="8c96f-173">Relationships</span></span>

| <span data-ttu-id="8c96f-174">Связь</span><span class="sxs-lookup"><span data-stu-id="8c96f-174">Relationship</span></span> | <span data-ttu-id="8c96f-175">Тип</span><span class="sxs-lookup"><span data-stu-id="8c96f-175">Type</span></span>        | <span data-ttu-id="8c96f-176">Описание</span><span class="sxs-lookup"><span data-stu-id="8c96f-176">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8c96f-177">Тег</span><span class="sxs-lookup"><span data-stu-id="8c96f-177">appliesTo</span></span>|<span data-ttu-id="8c96f-178">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="8c96f-178">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="8c96f-179">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="8c96f-179">Nullable.</span></span> <span data-ttu-id="8c96f-180">Указывает список Директорйобжектс, для которых включена функция.</span><span class="sxs-lookup"><span data-stu-id="8c96f-180">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8c96f-181">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="8c96f-181">JSON representation</span></span>

<span data-ttu-id="8c96f-182">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="8c96f-182">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "",
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


