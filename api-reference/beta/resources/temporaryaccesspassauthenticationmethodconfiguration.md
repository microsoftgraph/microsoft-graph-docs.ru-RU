---
title: Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration
description: Представляет политику методов проверки подлинности для временного прохода доступа.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9edb4038180a96d6878fcaf6770728a1befbca19
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272650"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="6a789-103">Тип ресурса temporaryAccessPassAuthenticationMethodConfiguration</span><span class="sxs-lookup"><span data-stu-id="6a789-103">temporaryAccessPassAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="6a789-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a789-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a789-105">Представляет политику методов проверки подлинности для временного прохода доступа.</span><span class="sxs-lookup"><span data-stu-id="6a789-105">Represents a Temporary Access Pass authentication methods policy.</span></span> <span data-ttu-id="6a789-106">Политика методов проверки подлинности определяет параметры конфигурации и пользователей или группы, которым включено использование метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6a789-106">The Authentication methods policy defines the configuration settings and users or groups who are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="6a789-107">Методы</span><span class="sxs-lookup"><span data-stu-id="6a789-107">Methods</span></span>
|<span data-ttu-id="6a789-108">Метод</span><span class="sxs-lookup"><span data-stu-id="6a789-108">Method</span></span>|<span data-ttu-id="6a789-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6a789-109">Return type</span></span>|<span data-ttu-id="6a789-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a789-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a789-111">[получение](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md);</span><span class="sxs-lookup"><span data-stu-id="6a789-111">[Get](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)</span></span>|[<span data-ttu-id="6a789-112">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="6a789-112">temporaryaccesspassauthenticationmethodconfiguration</span></span>](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="6a789-113">Чтение свойств и связей объекта **temporaryaccesspassauthenticationmethodconfiguration.**</span><span class="sxs-lookup"><span data-stu-id="6a789-113">Read the properties and relationships of a **temporaryaccesspassauthenticationmethodconfiguration** object.</span></span>|
|<span data-ttu-id="6a789-114">[обновление](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md).</span><span class="sxs-lookup"><span data-stu-id="6a789-114">[Update](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)</span></span>|[<span data-ttu-id="6a789-115">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="6a789-115">temporaryaccesspassauthenticationmethodconfiguration</span></span>](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="6a789-116">Обновление свойств объекта **temporaryaccesspassauthenticationmethodconfiguration.**</span><span class="sxs-lookup"><span data-stu-id="6a789-116">Update the properties of a **temporaryaccesspassauthenticationmethodconfiguration** object.</span></span>|
|<span data-ttu-id="6a789-117">[удаление](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md);</span><span class="sxs-lookup"><span data-stu-id="6a789-117">[Delete](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)</span></span>|<span data-ttu-id="6a789-118">Нет</span><span class="sxs-lookup"><span data-stu-id="6a789-118">None</span></span>|<span data-ttu-id="6a789-119">Возвращает объект **temporaryaccesspassauthenticationmethodconfiguration** в конфигурацию по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="6a789-119">Reverts the **temporaryaccesspassauthenticationmethodconfiguration** object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="6a789-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a789-120">Properties</span></span>
|<span data-ttu-id="6a789-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a789-121">Property</span></span>|<span data-ttu-id="6a789-122">Тип</span><span class="sxs-lookup"><span data-stu-id="6a789-122">Type</span></span>|<span data-ttu-id="6a789-123">Описание</span><span class="sxs-lookup"><span data-stu-id="6a789-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a789-124">id</span><span class="sxs-lookup"><span data-stu-id="6a789-124">id</span></span>|<span data-ttu-id="6a789-125">String</span><span class="sxs-lookup"><span data-stu-id="6a789-125">String</span></span>|<span data-ttu-id="6a789-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6a789-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="6a789-127">minimumLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="6a789-127">minimumLifetimeInMinutes</span></span>|<span data-ttu-id="6a789-128">Целое</span><span class="sxs-lookup"><span data-stu-id="6a789-128">Int</span></span>|<span data-ttu-id="6a789-129">Минимальный срок жизни (в минутах) для всех временныхaccessPass, созданных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6a789-129">Minimum lifetime in minutes for any temporaryAccessPass created in the tenant.</span></span> <span data-ttu-id="6a789-130">Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).</span><span class="sxs-lookup"><span data-stu-id="6a789-130">Value can be between 10 and 43200 minutes (equivalent to 30 days).</span></span>|
|<span data-ttu-id="6a789-131">maximumLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="6a789-131">maximumLifetimeInMinutes</span></span>|<span data-ttu-id="6a789-132">Целое</span><span class="sxs-lookup"><span data-stu-id="6a789-132">Int</span></span>|<span data-ttu-id="6a789-133">Максимальный срок действия в минутах для всех временныхaccessPass, созданных в клиенте.</span><span class="sxs-lookup"><span data-stu-id="6a789-133">Maximum lifetime in minutes for any temporaryAccessPass created in the tenant.</span></span> <span data-ttu-id="6a789-134">Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).</span><span class="sxs-lookup"><span data-stu-id="6a789-134">Value can be between 10 and 43200 minutes (equivalent to 30 days).</span></span>|
|<span data-ttu-id="6a789-135">defaultLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="6a789-135">defaultLifetimeInMinutes</span></span>|<span data-ttu-id="6a789-136">int</span><span class="sxs-lookup"><span data-stu-id="6a789-136">int</span></span>|<span data-ttu-id="6a789-137">Время жизни по умолчанию (в минутах) для temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="6a789-137">Default lifetime, in minutes, for a temporaryAccessPass.</span></span> <span data-ttu-id="6a789-138">Значение может быть между minimumLifetimeInMinutes и maximumLifetimeInMinutes.</span><span class="sxs-lookup"><span data-stu-id="6a789-138">Value can be between the minimumLifetimeInMinutes and maximumLifetimeInMinutes.</span></span>|
|<span data-ttu-id="6a789-139">defaultLength</span><span class="sxs-lookup"><span data-stu-id="6a789-139">defaultLength</span></span>|<span data-ttu-id="6a789-140">int</span><span class="sxs-lookup"><span data-stu-id="6a789-140">int</span></span>|<span data-ttu-id="6a789-141">Длина по умолчанию (в символах) временногоaccessPass от 8 до 48 символов.</span><span class="sxs-lookup"><span data-stu-id="6a789-141">Default length, in characters, of a temporaryAccessPass, between 8 and 48 characters.</span></span>|
|<span data-ttu-id="6a789-142">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="6a789-142">isUsableOnce</span></span>|<span data-ttu-id="6a789-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="6a789-143">Boolean</span></span>   |<span data-ttu-id="6a789-144">Если `true` все проходы в клиенте будут ограничены одновейным использованием.</span><span class="sxs-lookup"><span data-stu-id="6a789-144">If `true`, all the passes in the tenant will be restricted to one-time use.</span></span> <span data-ttu-id="6a789-145">Если , передается клиент может быть создан для `false` однократного или многократного использования.</span><span class="sxs-lookup"><span data-stu-id="6a789-145">If `false`, passes in the tenant can be created to be either one-time use or multiple time use.</span></span>|
|<span data-ttu-id="6a789-146">state</span><span class="sxs-lookup"><span data-stu-id="6a789-146">state</span></span>|<span data-ttu-id="6a789-147">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="6a789-147">authenticationMethodState</span></span>|<span data-ttu-id="6a789-148">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="6a789-148">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a789-149">Связи</span><span class="sxs-lookup"><span data-stu-id="6a789-149">Relationships</span></span>
|<span data-ttu-id="6a789-150">Связь</span><span class="sxs-lookup"><span data-stu-id="6a789-150">Relationship</span></span>|<span data-ttu-id="6a789-151">Тип</span><span class="sxs-lookup"><span data-stu-id="6a789-151">Type</span></span>|<span data-ttu-id="6a789-152">Описание</span><span class="sxs-lookup"><span data-stu-id="6a789-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a789-153">includeTargets</span><span class="sxs-lookup"><span data-stu-id="6a789-153">includeTargets</span></span>|<span data-ttu-id="6a789-154">[Коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="6a789-154">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="6a789-155">Коллекция пользователей или групп, которым включен метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="6a789-155">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6a789-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a789-156">JSON representation</span></span>
<span data-ttu-id="6a789-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6a789-157">The following is a JSON representation of the resource.</span></span>

``` json
{
  "@odata.type": "#microsoft.authMethodPolicy.temporaryAccessPassAuthenticationMethodConfiguration",
  "id": "String (identifier)",
  "state": "String",
  "defaultLifetimeInMinutes": "Integer",
  "defaultLength": "Integer",
  "minimumLifetimeInMinutes": "Integer",
  "maximumLifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean"
},
"includeTargets": [ { "@odata.type": "microsoft.graph.authenticationMethodTarget" } ]
}
```
