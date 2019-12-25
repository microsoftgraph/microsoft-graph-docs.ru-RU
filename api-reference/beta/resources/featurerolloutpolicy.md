---
title: Тип ресурса Феатурероллаутполици
description: Представляет политику развертывания компонентов, связанную с объектом каталога.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 958e6750c9b6a0749613d3a380b43a7d1ab282c2
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870252"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="21866-103">Тип ресурса Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-103">featureRolloutPolicy resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21866-104">Представляет политику развертывания компонентов, связанную с объектом каталога.</span><span class="sxs-lookup"><span data-stu-id="21866-104">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="21866-105">Создание политики развертывания компонентов поможет администраторам клиентов пилотно использовать определенную группу перед включением функций для всей Организации.</span><span class="sxs-lookup"><span data-stu-id="21866-105">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="21866-106">Это минимизирует воздействие и помогает администраторам постепенно тестировать и отменять связанные функции проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="21866-106">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="21866-107">Ниже приведены ограничения на развертывание функций.</span><span class="sxs-lookup"><span data-stu-id="21866-107">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="21866-108">Каждая функция поддерживает не более 10 групп.</span><span class="sxs-lookup"><span data-stu-id="21866-108">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="21866-109">Поле **appliesTo** поддерживает только группы.</span><span class="sxs-lookup"><span data-stu-id="21866-109">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="21866-110">Динамические группы и вложенные группы не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="21866-110">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="21866-111">Ниже приведены предварительные требования для каждой из функций, которые в настоящее время супортед для развертывания с помощью этой политики развертывания.</span><span class="sxs-lookup"><span data-stu-id="21866-111">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="21866-112">Сквозная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="21866-112">Passthrough Authentication</span></span>

* <span data-ttu-id="21866-113">Определите сервер под управлением Windows Server 2012 R2 или более поздней версии, на котором нужно запустить агент [пасссраугхаусентикатион](/azure/active-directory/hybrid/how-to-connect-pta) .</span><span class="sxs-lookup"><span data-stu-id="21866-113">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="21866-114">Убедитесь, что сервер присоединен к домену, может выполнять проверку подлинности выбранных пользователей с помощью Active Directory и может связываться с Azure AD на исходящих портах/URL-адресах.</span><span class="sxs-lookup"><span data-stu-id="21866-114"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="21866-115">[Скачайте](https://aka.ms/getauthagent) & установить агент проверки подлинности Microsoft Azure AD Connect на сервере.</span><span class="sxs-lookup"><span data-stu-id="21866-115">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="21866-116">Чтобы обеспечить высокий уровень доступности, установите дополнительные агенты проверки подлинности на других серверах, как описано [здесь](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span><span class="sxs-lookup"><span data-stu-id="21866-116">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="21866-117">Убедитесь, что параметры [интеллектуальной блокировки](/azure/active-directory/authentication/howto-password-smart-lockout) настроены соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="21866-117">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="21866-118">Это необходимо для того, чтобы локальные учетные записи пользователей Active Directory не блокировались с помощью недопустимых субъектов.</span><span class="sxs-lookup"><span data-stu-id="21866-118">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="21866-119">сеамлессссо</span><span class="sxs-lookup"><span data-stu-id="21866-119">SeamlessSso</span></span>

* <span data-ttu-id="21866-120">Включите [сеамлессссо](/azure/active-directory/hybrid/how-to-connect-sso) для лесов Active Directory в соответствии с [этими](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) инструкциями.</span><span class="sxs-lookup"><span data-stu-id="21866-120">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="21866-121">пассвордхашсинк</span><span class="sxs-lookup"><span data-stu-id="21866-121">PasswordHashSync</span></span>

* <span data-ttu-id="21866-122">Включите [пассвордхашсинк](/azure/active-directory/hybrid/whatis-phs) на странице "дополнительные компоненты" в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="21866-122">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

## <a name="methods"></a><span data-ttu-id="21866-123">Методы</span><span class="sxs-lookup"><span data-stu-id="21866-123">Methods</span></span>

| <span data-ttu-id="21866-124">Метод</span><span class="sxs-lookup"><span data-stu-id="21866-124">Method</span></span>       | <span data-ttu-id="21866-125">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="21866-125">Return Type</span></span> | <span data-ttu-id="21866-126">Описание</span><span class="sxs-lookup"><span data-stu-id="21866-126">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="21866-127">Список ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="21866-127">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="21866-128">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-128">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="21866-129">Получение списка объектов Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="21866-129">Retrieve a list of featureRolloutPolicy objects.</span></span> |
| [<span data-ttu-id="21866-130">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-130">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="21866-131">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-131">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="21866-132">Получение свойств и связей объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="21866-132">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> ||
| [<span data-ttu-id="21866-133">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-133">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="21866-134">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-134">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="21866-135">Создание нового объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="21866-135">Create a new featureRolloutPolicy object.</span></span>
| [<span data-ttu-id="21866-136">Обновление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-136">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="21866-137">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-137">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="21866-138">Обновление свойств объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="21866-138">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="21866-139">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="21866-139">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="21866-140">Нет.</span><span class="sxs-lookup"><span data-stu-id="21866-140">None</span></span> | <span data-ttu-id="21866-141">Удаление объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="21866-141">Delete a featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="21866-142">Назначение appliesTo</span><span class="sxs-lookup"><span data-stu-id="21866-142">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md) | [<span data-ttu-id="21866-143">directoryObject</span><span class="sxs-lookup"><span data-stu-id="21866-143">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="21866-144">Назначение directoryObject для развертывания компонентов.</span><span class="sxs-lookup"><span data-stu-id="21866-144">Assign a directoryObject to feature rollout.</span></span> |
| [<span data-ttu-id="21866-145">Удаление appliesTo</span><span class="sxs-lookup"><span data-stu-id="21866-145">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md) | <span data-ttu-id="21866-146">Нет.</span><span class="sxs-lookup"><span data-stu-id="21866-146">None</span></span> | <span data-ttu-id="21866-147">Удаление directoryObject из развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="21866-147">Remove a directoryObject from feature rollout.</span></span> |

## <a name="properties"></a><span data-ttu-id="21866-148">Свойства</span><span class="sxs-lookup"><span data-stu-id="21866-148">Properties</span></span>

| <span data-ttu-id="21866-149">Свойство</span><span class="sxs-lookup"><span data-stu-id="21866-149">Property</span></span>     | <span data-ttu-id="21866-150">Тип</span><span class="sxs-lookup"><span data-stu-id="21866-150">Type</span></span>        | <span data-ttu-id="21866-151">Описание</span><span class="sxs-lookup"><span data-stu-id="21866-151">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21866-152">description</span><span class="sxs-lookup"><span data-stu-id="21866-152">description</span></span>|<span data-ttu-id="21866-153">String</span><span class="sxs-lookup"><span data-stu-id="21866-153">String</span></span>|<span data-ttu-id="21866-154">Описание этой политики развертывания функций.</span><span class="sxs-lookup"><span data-stu-id="21866-154">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="21866-155">displayName</span><span class="sxs-lookup"><span data-stu-id="21866-155">displayName</span></span>|<span data-ttu-id="21866-156">Строка</span><span class="sxs-lookup"><span data-stu-id="21866-156">String</span></span>|<span data-ttu-id="21866-157">Отображаемое имя для этой политики развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="21866-157">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="21866-158">состав</span><span class="sxs-lookup"><span data-stu-id="21866-158">feature</span></span>|<span data-ttu-id="21866-159">стажедфеатуренаме</span><span class="sxs-lookup"><span data-stu-id="21866-159">stagedFeatureName</span></span>| <span data-ttu-id="21866-160">Возможные значения: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="21866-160">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="21866-161">id</span><span class="sxs-lookup"><span data-stu-id="21866-161">id</span></span>|<span data-ttu-id="21866-162">String</span><span class="sxs-lookup"><span data-stu-id="21866-162">String</span></span>| <span data-ttu-id="21866-163">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="21866-163">Read-only.</span></span>|
|<span data-ttu-id="21866-164">исапплиедтурганизатион</span><span class="sxs-lookup"><span data-stu-id="21866-164">isAppliedToOrganization</span></span>|<span data-ttu-id="21866-165">Логический</span><span class="sxs-lookup"><span data-stu-id="21866-165">Boolean</span></span>|<span data-ttu-id="21866-166">Указывает, следует ли применять эту политику развертывания функций ко всей Организации.</span><span class="sxs-lookup"><span data-stu-id="21866-166">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="21866-167">isEnabled</span><span class="sxs-lookup"><span data-stu-id="21866-167">isEnabled</span></span>|<span data-ttu-id="21866-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="21866-168">Boolean</span></span>|<span data-ttu-id="21866-169">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="21866-169">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="21866-170">Отношения</span><span class="sxs-lookup"><span data-stu-id="21866-170">Relationships</span></span>

| <span data-ttu-id="21866-171">Связь</span><span class="sxs-lookup"><span data-stu-id="21866-171">Relationship</span></span> | <span data-ttu-id="21866-172">Тип</span><span class="sxs-lookup"><span data-stu-id="21866-172">Type</span></span>        | <span data-ttu-id="21866-173">Описание</span><span class="sxs-lookup"><span data-stu-id="21866-173">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="21866-174">Тег</span><span class="sxs-lookup"><span data-stu-id="21866-174">appliesTo</span></span>|<span data-ttu-id="21866-175">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="21866-175">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="21866-176">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="21866-176">Nullable.</span></span> <span data-ttu-id="21866-177">Указывает список Директорйобжектс, для которых включена функция.</span><span class="sxs-lookup"><span data-stu-id="21866-177">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21866-178">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="21866-178">JSON representation</span></span>

<span data-ttu-id="21866-179">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="21866-179">The following is a JSON representation of the resource.</span></span>

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
