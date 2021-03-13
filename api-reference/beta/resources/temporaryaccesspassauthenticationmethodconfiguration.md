---
title: temporaryAccessPassAuthenticationMethodConfiguration resource type
description: Представляет политику методов проверки подлинности с временным пропуском доступа.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: apiPageType
ms.openlocfilehash: ccdb139beff0019e9cad3f6c4e223369f9c6e66e
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760969"
---
# <a name="temporaryaccesspassauthenticationmethodconfiguration-resource-type"></a><span data-ttu-id="10532-103">temporaryAccessPassAuthenticationMethodConfiguration resource type</span><span class="sxs-lookup"><span data-stu-id="10532-103">temporaryAccessPassAuthenticationMethodConfiguration resource type</span></span>
<span data-ttu-id="10532-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10532-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10532-105">Представляет политику методов проверки подлинности с временным пропуском доступа.</span><span class="sxs-lookup"><span data-stu-id="10532-105">Represents a Temporary Access Pass authentication methods policy.</span></span> <span data-ttu-id="10532-106">Политика методов проверки подлинности определяет параметры конфигурации и пользователей или групп, которым включен метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="10532-106">The Authentication methods policy defines the configuration settings and users or groups who are enabled to use the authentication method.</span></span>

## <a name="methods"></a><span data-ttu-id="10532-107">Методы</span><span class="sxs-lookup"><span data-stu-id="10532-107">Methods</span></span>
|<span data-ttu-id="10532-108">Метод</span><span class="sxs-lookup"><span data-stu-id="10532-108">Method</span></span>|<span data-ttu-id="10532-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="10532-109">Return type</span></span>|<span data-ttu-id="10532-110">Описание</span><span class="sxs-lookup"><span data-stu-id="10532-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10532-111">[получение](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md);</span><span class="sxs-lookup"><span data-stu-id="10532-111">[Get](../api/temporaryaccesspassauthenticationmethodconfiguration-get.md)</span></span>|[<span data-ttu-id="10532-112">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="10532-112">temporaryaccesspassauthenticationmethodconfiguration</span></span>](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="10532-113">Ознакомьтесь с свойствами и отношениями объекта **temporaryaccesspassauthenticationmethodconfiguration.**</span><span class="sxs-lookup"><span data-stu-id="10532-113">Read the properties and relationships of a **temporaryaccesspassauthenticationmethodconfiguration** object.</span></span>|
|[<span data-ttu-id="10532-114">Update</span><span class="sxs-lookup"><span data-stu-id="10532-114">Update</span></span>](../api/temporaryaccesspassauthenticationmethodconfiguration-update.md)|[<span data-ttu-id="10532-115">temporaryaccesspassauthenticationmethodconfiguration</span><span class="sxs-lookup"><span data-stu-id="10532-115">temporaryaccesspassauthenticationmethodconfiguration</span></span>](../resources/temporaryaccesspassauthenticationmethodconfiguration.md)|<span data-ttu-id="10532-116">Обновление свойств объекта **temporaryaccesspassauthenticationmethodconfiguration.**</span><span class="sxs-lookup"><span data-stu-id="10532-116">Update the properties of a **temporaryaccesspassauthenticationmethodconfiguration** object.</span></span>|
|[<span data-ttu-id="10532-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="10532-117">Delete</span></span>](../api/temporaryaccesspassauthenticationmethodconfiguration-delete.md)|<span data-ttu-id="10532-118">Нет</span><span class="sxs-lookup"><span data-stu-id="10532-118">None</span></span>|<span data-ttu-id="10532-119">Возвращает объект **temporaryaccesspassauthenticationmethodconfiguration** к конфигурации по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="10532-119">Reverts the **temporaryaccesspassauthenticationmethodconfiguration** object to its default configuration.</span></span>|

## <a name="properties"></a><span data-ttu-id="10532-120">Свойства</span><span class="sxs-lookup"><span data-stu-id="10532-120">Properties</span></span>
|<span data-ttu-id="10532-121">Свойство</span><span class="sxs-lookup"><span data-stu-id="10532-121">Property</span></span>|<span data-ttu-id="10532-122">Тип</span><span class="sxs-lookup"><span data-stu-id="10532-122">Type</span></span>|<span data-ttu-id="10532-123">Описание</span><span class="sxs-lookup"><span data-stu-id="10532-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10532-124">id</span><span class="sxs-lookup"><span data-stu-id="10532-124">id</span></span>|<span data-ttu-id="10532-125">String</span><span class="sxs-lookup"><span data-stu-id="10532-125">String</span></span>|<span data-ttu-id="10532-126">Идентификатор политики метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="10532-126">The authentication method policy identifier.</span></span>|
|<span data-ttu-id="10532-127">minimumLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="10532-127">minimumLifetimeInMinutes</span></span>|<span data-ttu-id="10532-128">Целое</span><span class="sxs-lookup"><span data-stu-id="10532-128">Int</span></span>|<span data-ttu-id="10532-129">Минимальный срок службы в минутах для любого временногоAccessPass, созданного в клиенте.</span><span class="sxs-lookup"><span data-stu-id="10532-129">Minimum lifetime in minutes for any temporaryAccessPass created in the tenant.</span></span> <span data-ttu-id="10532-130">Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).</span><span class="sxs-lookup"><span data-stu-id="10532-130">Value can be between 10 and 43200 minutes (equivalent to 30 days).</span></span>|
|<span data-ttu-id="10532-131">maximumLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="10532-131">maximumLifetimeInMinutes</span></span>|<span data-ttu-id="10532-132">Целое</span><span class="sxs-lookup"><span data-stu-id="10532-132">Int</span></span>|<span data-ttu-id="10532-133">Максимальный срок службы в минутах для любого временногоAccessPass, созданного в клиенте.</span><span class="sxs-lookup"><span data-stu-id="10532-133">Maximum lifetime in minutes for any temporaryAccessPass created in the tenant.</span></span> <span data-ttu-id="10532-134">Значение может быть от 10 до 43200 минут (эквивалентно 30 дням).</span><span class="sxs-lookup"><span data-stu-id="10532-134">Value can be between 10 and 43200 minutes (equivalent to 30 days).</span></span>|
|<span data-ttu-id="10532-135">defaultLifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="10532-135">defaultLifetimeInMinutes</span></span>|<span data-ttu-id="10532-136">int</span><span class="sxs-lookup"><span data-stu-id="10532-136">int</span></span>|<span data-ttu-id="10532-137">Срок службы по умолчанию в минутах для временногоAccessPass.</span><span class="sxs-lookup"><span data-stu-id="10532-137">Default lifetime, in minutes, for a temporaryAccessPass.</span></span> <span data-ttu-id="10532-138">Значение может быть между минимумомLifetimeInMinutes и maximumLifetimeInMinutes.</span><span class="sxs-lookup"><span data-stu-id="10532-138">Value can be between the minimumLifetimeInMinutes and maximumLifetimeInMinutes.</span></span>|
|<span data-ttu-id="10532-139">defaultLength</span><span class="sxs-lookup"><span data-stu-id="10532-139">defaultLength</span></span>|<span data-ttu-id="10532-140">int</span><span class="sxs-lookup"><span data-stu-id="10532-140">int</span></span>|<span data-ttu-id="10532-141">Длина по умолчанию в символах временногоAccessPass составляет от 8 до 48 символов.</span><span class="sxs-lookup"><span data-stu-id="10532-141">Default length, in characters, of a temporaryAccessPass, between 8 and 48 characters.</span></span>|
|<span data-ttu-id="10532-142">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="10532-142">isUsableOnce</span></span>|<span data-ttu-id="10532-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="10532-143">Boolean</span></span>   |<span data-ttu-id="10532-144">Если все пропуска в клиенте будут ограничены `true` одновековой помощью.</span><span class="sxs-lookup"><span data-stu-id="10532-144">If `true`, all the passes in the tenant will be restricted to one-time use.</span></span> <span data-ttu-id="10532-145">Если в клиенте может быть создано однократное использование или `false` многократное использование времени.</span><span class="sxs-lookup"><span data-stu-id="10532-145">If `false`, passes in the tenant can be created to be either one-time use or multiple time use.</span></span>|
|<span data-ttu-id="10532-146">state</span><span class="sxs-lookup"><span data-stu-id="10532-146">state</span></span>|<span data-ttu-id="10532-147">authenticationMethodState</span><span class="sxs-lookup"><span data-stu-id="10532-147">authenticationMethodState</span></span>|<span data-ttu-id="10532-148">Возможные значения: `enabled`, `disabled`.</span><span class="sxs-lookup"><span data-stu-id="10532-148">Possible values are: `enabled`, `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="10532-149">Отношения</span><span class="sxs-lookup"><span data-stu-id="10532-149">Relationships</span></span>
|<span data-ttu-id="10532-150">Связь</span><span class="sxs-lookup"><span data-stu-id="10532-150">Relationship</span></span>|<span data-ttu-id="10532-151">Тип</span><span class="sxs-lookup"><span data-stu-id="10532-151">Type</span></span>|<span data-ttu-id="10532-152">Описание</span><span class="sxs-lookup"><span data-stu-id="10532-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10532-153">includeTargets</span><span class="sxs-lookup"><span data-stu-id="10532-153">includeTargets</span></span>|<span data-ttu-id="10532-154">[коллекция authenticationMethodTarget](../resources/authenticationmethodtarget.md)</span><span class="sxs-lookup"><span data-stu-id="10532-154">[authenticationMethodTarget](../resources/authenticationmethodtarget.md) collection</span></span>|<span data-ttu-id="10532-155">Коллекция пользователей или групп, которые могут использовать метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="10532-155">A collection of users or groups who are enabled to use the authentication method.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="10532-156">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="10532-156">JSON representation</span></span>
<span data-ttu-id="10532-157">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10532-157">The following is a JSON representation of the resource.</span></span>

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
