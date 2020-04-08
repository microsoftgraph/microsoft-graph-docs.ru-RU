---
title: Тип ресурса Феатурероллаутполици
description: Представляет политику развертывания компонентов, связанную с объектом каталога.
localization_priority: Normal
author: keylimesoda
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 27e421283c9908c648769ccbe652f990f2728fce
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181724"
---
# <a name="featurerolloutpolicy-resource-type"></a><span data-ttu-id="822f5-103">Тип ресурса Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-103">featureRolloutPolicy resource type</span></span>

<span data-ttu-id="822f5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="822f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="822f5-105">Представляет политику развертывания компонентов, связанную с объектом каталога.</span><span class="sxs-lookup"><span data-stu-id="822f5-105">Represents a feature rollout policy associated with a directory object.</span></span> <span data-ttu-id="822f5-106">Создание политики развертывания компонентов поможет администраторам клиентов пилотно использовать определенную группу перед включением функций для всей Организации.</span><span class="sxs-lookup"><span data-stu-id="822f5-106">Creating a feature rollout policy helps tenant administrators to pilot features of Azure AD with a specific group before enabling features for entire organization.</span></span> <span data-ttu-id="822f5-107">Это минимизирует воздействие и помогает администраторам постепенно тестировать и отменять связанные функции проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="822f5-107">This minimizes the impact and helps administrators to test and rollout authentication related features gradually.</span></span>

<span data-ttu-id="822f5-108">Ниже приведены ограничения на развертывание функций.</span><span class="sxs-lookup"><span data-stu-id="822f5-108">The following are limitations of feature rollout:</span></span>

- <span data-ttu-id="822f5-109">Каждая функция поддерживает не более 10 групп.</span><span class="sxs-lookup"><span data-stu-id="822f5-109">Each feature supports a maximum of 10 groups.</span></span>
- <span data-ttu-id="822f5-110">Поле **appliesTo** поддерживает только группы.</span><span class="sxs-lookup"><span data-stu-id="822f5-110">The **appliesTo** field only supports groups.</span></span>
- <span data-ttu-id="822f5-111">Динамические группы и вложенные группы не поддерживаются.</span><span class="sxs-lookup"><span data-stu-id="822f5-111">Dynamic groups and nested groups are not supported.</span></span>

<span data-ttu-id="822f5-112">Ниже приведены предварительные требования для каждой из функций, которые в настоящее время супортед для развертывания с помощью этой политики развертывания.</span><span class="sxs-lookup"><span data-stu-id="822f5-112">The following are pre-requisites for each of the features that are currently suported for rollout using this rollout policy.</span></span>

### <a name="passthrough-authentication"></a><span data-ttu-id="822f5-113">Сквозная проверка подлинности</span><span class="sxs-lookup"><span data-stu-id="822f5-113">Passthrough Authentication</span></span>

* <span data-ttu-id="822f5-114">Определите сервер под управлением Windows Server 2012 R2 или более поздней версии, на котором нужно запустить агент [пасссраугхаусентикатион](/azure/active-directory/hybrid/how-to-connect-pta) .</span><span class="sxs-lookup"><span data-stu-id="822f5-114">Identify a server running Windows Server 2012 R2 or later where you want the [PassthroughAuthentication](/azure/active-directory/hybrid/how-to-connect-pta) Agent to run.</span></span><span data-ttu-id="822f5-115">Убедитесь, что сервер присоединен к домену, может выполнять проверку подлинности выбранных пользователей с помощью Active Directory и может связываться с Azure AD на исходящих портах/URL-адресах.</span><span class="sxs-lookup"><span data-stu-id="822f5-115"> Ensure that the server is domain-joined, can authenticate selected users with Active Directory, and can communicate with Azure AD on outbound ports / URLs.</span></span>
* <span data-ttu-id="822f5-116">[Скачайте](https://aka.ms/getauthagent) & установить агент проверки подлинности Microsoft Azure AD Connect на сервере.</span><span class="sxs-lookup"><span data-stu-id="822f5-116">[Download](https://aka.ms/getauthagent) & install the Microsoft Azure AD Connect Authentication Agent on the server.</span></span>
* <span data-ttu-id="822f5-117">Чтобы обеспечить высокий уровень доступности, установите дополнительные агенты проверки подлинности на других серверах, как описано [здесь](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span><span class="sxs-lookup"><span data-stu-id="822f5-117">To enable high availability, install additional Authentication Agents on other servers as described [here](/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability).</span></span>
* <span data-ttu-id="822f5-118">Убедитесь, что параметры [интеллектуальной блокировки](/azure/active-directory/authentication/howto-password-smart-lockout) настроены соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="822f5-118">Ensure that you have configured your [Smart Lockout](/azure/active-directory/authentication/howto-password-smart-lockout) settings appropriately.</span></span> <span data-ttu-id="822f5-119">Это необходимо для того, чтобы локальные учетные записи пользователей Active Directory не блокировались с помощью недопустимых субъектов.</span><span class="sxs-lookup"><span data-stu-id="822f5-119">This is to ensure that your users’ on-premises Active Directory accounts don’t get locked out by bad actors.</span></span>

### <a name="seamlesssso"></a><span data-ttu-id="822f5-120">сеамлессссо</span><span class="sxs-lookup"><span data-stu-id="822f5-120">SeamlessSso</span></span>

* <span data-ttu-id="822f5-121">Включите [сеамлессссо](/azure/active-directory/hybrid/how-to-connect-sso) для лесов Active Directory в соответствии с [этими](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) инструкциями.</span><span class="sxs-lookup"><span data-stu-id="822f5-121">Enable [SeamlessSso](/azure/active-directory/hybrid/how-to-connect-sso) for the AD forests based on [these](/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature) instructions.</span></span>

### <a name="passwordhashsync"></a><span data-ttu-id="822f5-122">пассвордхашсинк</span><span class="sxs-lookup"><span data-stu-id="822f5-122">PasswordHashSync</span></span>

* <span data-ttu-id="822f5-123">Включите [пассвордхашсинк](/azure/active-directory/hybrid/whatis-phs) на странице "дополнительные компоненты" в Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="822f5-123">Enable [PasswordHashSync](/azure/active-directory/hybrid/whatis-phs) from the “Optional features” page in Azure AD Connect.</span></span>

## <a name="methods"></a><span data-ttu-id="822f5-124">Методы</span><span class="sxs-lookup"><span data-stu-id="822f5-124">Methods</span></span>

| <span data-ttu-id="822f5-125">Метод</span><span class="sxs-lookup"><span data-stu-id="822f5-125">Method</span></span>       | <span data-ttu-id="822f5-126">Возвращаемый тип</span><span class="sxs-lookup"><span data-stu-id="822f5-126">Return Type</span></span> | <span data-ttu-id="822f5-127">Описание</span><span class="sxs-lookup"><span data-stu-id="822f5-127">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="822f5-128">Список ФеатурероллаутполиЦиес</span><span class="sxs-lookup"><span data-stu-id="822f5-128">List featureRolloutPolicies</span></span>](../api/directory-list-featurerolloutpolicies.md) | [<span data-ttu-id="822f5-129">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-129">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="822f5-130">Получение списка объектов Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="822f5-130">Retrieve a list of featureRolloutPolicy objects.</span></span> |
| [<span data-ttu-id="822f5-131">Получение Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-131">Get featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-get.md) | [<span data-ttu-id="822f5-132">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-132">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="822f5-133">Получение свойств и связей объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="822f5-133">Retrieve the properties and relationships of featurerolloutpolicy object.</span></span> ||
| [<span data-ttu-id="822f5-134">Создание Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-134">Create featureRolloutPolicy</span></span>](../api/directory-post-featurerolloutpolicies.md) | [<span data-ttu-id="822f5-135">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-135">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="822f5-136">Создание нового объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="822f5-136">Create a new featureRolloutPolicy object.</span></span>
| [<span data-ttu-id="822f5-137">Обновление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-137">Update featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-update.md) | [<span data-ttu-id="822f5-138">феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-138">featureRolloutPolicy</span></span>](featurerolloutpolicy.md) | <span data-ttu-id="822f5-139">Обновление свойств объекта феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="822f5-139">Update the properties of featurerolloutpolicy object.</span></span> |
| [<span data-ttu-id="822f5-140">Удаление Феатурероллаутполици</span><span class="sxs-lookup"><span data-stu-id="822f5-140">Delete featureRolloutPolicy</span></span>](../api/featurerolloutpolicy-delete.md) | <span data-ttu-id="822f5-141">Нет</span><span class="sxs-lookup"><span data-stu-id="822f5-141">None</span></span> | <span data-ttu-id="822f5-142">Удаление объекта Феатурероллаутполици.</span><span class="sxs-lookup"><span data-stu-id="822f5-142">Delete a featureRolloutPolicy object.</span></span> |
| [<span data-ttu-id="822f5-143">Назначение appliesTo</span><span class="sxs-lookup"><span data-stu-id="822f5-143">Assign appliesTo</span></span>](../api/featurerolloutpolicy-post-appliesto.md) | [<span data-ttu-id="822f5-144">directoryObject</span><span class="sxs-lookup"><span data-stu-id="822f5-144">directoryObject</span></span>](directoryobject.md) | <span data-ttu-id="822f5-145">Назначение directoryObject для развертывания компонентов.</span><span class="sxs-lookup"><span data-stu-id="822f5-145">Assign a directoryObject to feature rollout.</span></span> |
| [<span data-ttu-id="822f5-146">Удаление appliesTo</span><span class="sxs-lookup"><span data-stu-id="822f5-146">Remove appliesTo</span></span>](../api/featurerolloutpolicy-delete-appliesto.md) | <span data-ttu-id="822f5-147">Нет</span><span class="sxs-lookup"><span data-stu-id="822f5-147">None</span></span> | <span data-ttu-id="822f5-148">Удаление directoryObject из развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="822f5-148">Remove a directoryObject from feature rollout.</span></span> |

## <a name="properties"></a><span data-ttu-id="822f5-149">Свойства</span><span class="sxs-lookup"><span data-stu-id="822f5-149">Properties</span></span>

| <span data-ttu-id="822f5-150">Свойство</span><span class="sxs-lookup"><span data-stu-id="822f5-150">Property</span></span>     | <span data-ttu-id="822f5-151">Тип</span><span class="sxs-lookup"><span data-stu-id="822f5-151">Type</span></span>        | <span data-ttu-id="822f5-152">Описание</span><span class="sxs-lookup"><span data-stu-id="822f5-152">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="822f5-153">description</span><span class="sxs-lookup"><span data-stu-id="822f5-153">description</span></span>|<span data-ttu-id="822f5-154">String</span><span class="sxs-lookup"><span data-stu-id="822f5-154">String</span></span>|<span data-ttu-id="822f5-155">Описание этой политики развертывания функций.</span><span class="sxs-lookup"><span data-stu-id="822f5-155">A description for this feature rollout policy.</span></span>|
|<span data-ttu-id="822f5-156">displayName</span><span class="sxs-lookup"><span data-stu-id="822f5-156">displayName</span></span>|<span data-ttu-id="822f5-157">Строка</span><span class="sxs-lookup"><span data-stu-id="822f5-157">String</span></span>|<span data-ttu-id="822f5-158">Отображаемое имя для этой политики развертывания компонента.</span><span class="sxs-lookup"><span data-stu-id="822f5-158">The display name for this  feature rollout policy.</span></span>|
|<span data-ttu-id="822f5-159">состав</span><span class="sxs-lookup"><span data-stu-id="822f5-159">feature</span></span>|<span data-ttu-id="822f5-160">стажедфеатуренаме</span><span class="sxs-lookup"><span data-stu-id="822f5-160">stagedFeatureName</span></span>| <span data-ttu-id="822f5-161">Возможные значения: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="822f5-161">Possible values are: `passthroughAuthentication`, `seamlessSso`, `passwordHashSync`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="822f5-162">id</span><span class="sxs-lookup"><span data-stu-id="822f5-162">id</span></span>|<span data-ttu-id="822f5-163">String</span><span class="sxs-lookup"><span data-stu-id="822f5-163">String</span></span>| <span data-ttu-id="822f5-164">Только для чтения.</span><span class="sxs-lookup"><span data-stu-id="822f5-164">Read-only.</span></span>|
|<span data-ttu-id="822f5-165">исапплиедтурганизатион</span><span class="sxs-lookup"><span data-stu-id="822f5-165">isAppliedToOrganization</span></span>|<span data-ttu-id="822f5-166">Логический</span><span class="sxs-lookup"><span data-stu-id="822f5-166">Boolean</span></span>|<span data-ttu-id="822f5-167">Указывает, следует ли применять эту политику развертывания функций ко всей Организации.</span><span class="sxs-lookup"><span data-stu-id="822f5-167">Indicates whether this feature rollout policy should be applied to the entire organization.</span></span>|
|<span data-ttu-id="822f5-168">isEnabled</span><span class="sxs-lookup"><span data-stu-id="822f5-168">isEnabled</span></span>|<span data-ttu-id="822f5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="822f5-169">Boolean</span></span>|<span data-ttu-id="822f5-170">Указывает, включен ли выпуск компонентов.</span><span class="sxs-lookup"><span data-stu-id="822f5-170">Indicates whether the feature rollout is enabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="822f5-171">Отношения</span><span class="sxs-lookup"><span data-stu-id="822f5-171">Relationships</span></span>

| <span data-ttu-id="822f5-172">Связь</span><span class="sxs-lookup"><span data-stu-id="822f5-172">Relationship</span></span> | <span data-ttu-id="822f5-173">Тип</span><span class="sxs-lookup"><span data-stu-id="822f5-173">Type</span></span>        | <span data-ttu-id="822f5-174">Описание</span><span class="sxs-lookup"><span data-stu-id="822f5-174">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="822f5-175">Тег</span><span class="sxs-lookup"><span data-stu-id="822f5-175">appliesTo</span></span>|<span data-ttu-id="822f5-176">Коллекция [directoryObject](directoryobject.md)</span><span class="sxs-lookup"><span data-stu-id="822f5-176">[directoryObject](directoryobject.md) collection</span></span>| <span data-ttu-id="822f5-177">Допускается значение null.</span><span class="sxs-lookup"><span data-stu-id="822f5-177">Nullable.</span></span> <span data-ttu-id="822f5-178">Указывает список Директорйобжектс, для которых включена функция.</span><span class="sxs-lookup"><span data-stu-id="822f5-178">Specifies a list of directoryObjects that feature is enabled for.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="822f5-179">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="822f5-179">JSON representation</span></span>

<span data-ttu-id="822f5-180">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="822f5-180">The following is a JSON representation of the resource.</span></span>

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
