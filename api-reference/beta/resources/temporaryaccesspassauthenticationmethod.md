---
title: Тип ресурса temporaryAccessPassAuthenticationMethod
description: Представляет временный проход доступа, зарегистрированный для пользователя.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e7e0afc084106face2ef8726f3273638d1a8eec0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272653"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a><span data-ttu-id="fd1db-103">Тип ресурса temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fd1db-103">temporaryAccessPassAuthenticationMethod resource type</span></span>

<span data-ttu-id="fd1db-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd1db-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd1db-105">Представляет временный доступ, зарегистрированный для пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd1db-105">Represents a Temporaty Access Pass registered to a user.</span></span> <span data-ttu-id="fd1db-106">Временный пароль — это ограниченный по времени пароль, который служит в качестве надежных учетных данных и позволяет вводить учетные данные без пароля.</span><span class="sxs-lookup"><span data-stu-id="fd1db-106">A Temporary Access Pass is a time-limited passcode that serves as a strong credential and allows onboarding of passwordless credentials.</span></span>

## <a name="methods"></a><span data-ttu-id="fd1db-107">Методы</span><span class="sxs-lookup"><span data-stu-id="fd1db-107">Methods</span></span>
|<span data-ttu-id="fd1db-108">Метод</span><span class="sxs-lookup"><span data-stu-id="fd1db-108">Method</span></span>|<span data-ttu-id="fd1db-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="fd1db-109">Return type</span></span>|<span data-ttu-id="fd1db-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fd1db-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fd1db-111">Список</span><span class="sxs-lookup"><span data-stu-id="fd1db-111">List</span></span>](../api/temporaryaccesspassauthenticationmethod-list.md)|<span data-ttu-id="fd1db-112">[коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="fd1db-112">[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) collection</span></span>|<span data-ttu-id="fd1db-113">Получить список временных **объектовAccessPassAuthenticationMethod** пользователя и их свойств.</span><span class="sxs-lookup"><span data-stu-id="fd1db-113">Retrieve a list of a user's **temporaryAccessPassAuthenticationMethod** objects and their properties.</span></span> <span data-ttu-id="fd1db-114">У пользователей может быть только один метод проверки подлинности с временным доступом.</span><span class="sxs-lookup"><span data-stu-id="fd1db-114">Users can only have one Temporary Access Pass authentication method.</span></span>|
|[<span data-ttu-id="fd1db-115">Создание</span><span class="sxs-lookup"><span data-stu-id="fd1db-115">Create</span></span>](../api/temporaryaccesspassauthenticationmethod-post.md)|[<span data-ttu-id="fd1db-116">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fd1db-116">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="fd1db-117">Создание объекта **temporaryAccessPassAuthenticationMethod** пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd1db-117">Create a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|
|<span data-ttu-id="fd1db-118">[получение](../api/temporaryaccesspassauthenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="fd1db-118">[Get](../api/temporaryaccesspassauthenticationmethod-get.md)</span></span>|[<span data-ttu-id="fd1db-119">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="fd1db-119">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="fd1db-120">Извлечение свойств временного объекта **UserAccessPassAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="fd1db-120">Retrieve the properties of the user's **temporaryAccessPassAuthenticationMethod** object.</span></span>||
|<span data-ttu-id="fd1db-121">[удаление](../api/temporaryaccesspassauthenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="fd1db-121">[Delete](../api/temporaryaccesspassauthenticationmethod-delete.md)</span></span>|<span data-ttu-id="fd1db-122">Нет</span><span class="sxs-lookup"><span data-stu-id="fd1db-122">None</span></span>|<span data-ttu-id="fd1db-123">Удаление объекта **temporaryAccessPassAuthenticationMethod** пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd1db-123">Delete a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fd1db-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="fd1db-124">Properties</span></span>
|<span data-ttu-id="fd1db-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="fd1db-125">Property</span></span>|<span data-ttu-id="fd1db-126">Тип</span><span class="sxs-lookup"><span data-stu-id="fd1db-126">Type</span></span>|<span data-ttu-id="fd1db-127">Описание</span><span class="sxs-lookup"><span data-stu-id="fd1db-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd1db-128">id</span><span class="sxs-lookup"><span data-stu-id="fd1db-128">id</span></span>|<span data-ttu-id="fd1db-129">String</span><span class="sxs-lookup"><span data-stu-id="fd1db-129">String</span></span>|<span data-ttu-id="fd1db-130">Идентификатор временного доступа, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="fd1db-130">The identifier of the Temporary Access Pass registered to this user.</span></span>|
|<span data-ttu-id="fd1db-131">temporaryAccessPass</span><span class="sxs-lookup"><span data-stu-id="fd1db-131">temporaryAccessPass</span></span>|<span data-ttu-id="fd1db-132">String</span><span class="sxs-lookup"><span data-stu-id="fd1db-132">String</span></span>|<span data-ttu-id="fd1db-133">ВременныйaccessPass, используемый для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="fd1db-133">The temporaryAccessPass used to authenticate.</span></span> <span data-ttu-id="fd1db-134">Возвращается только при создании нового временногоaccessPass; возвращается как NULL с get.</span><span class="sxs-lookup"><span data-stu-id="fd1db-134">Returned only on creation of a new temporaryAccessPass; returned as NULL with GET.</span></span>|
|<span data-ttu-id="fd1db-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fd1db-135">createdDateTime</span></span>|<span data-ttu-id="fd1db-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd1db-136">DateTimeOffset</span></span>|<span data-ttu-id="fd1db-137">Дата и время создания temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="fd1db-137">The date and time when the temporaryAccessPass was created.</span></span>|
|<span data-ttu-id="fd1db-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="fd1db-138">startDateTime</span></span>|<span data-ttu-id="fd1db-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd1db-139">DateTimeOffset</span></span>|<span data-ttu-id="fd1db-140">Дата и время, когда временныйaccessPass становится доступным для использования.</span><span class="sxs-lookup"><span data-stu-id="fd1db-140">The date and time when the temporaryAccessPass becomes available to use.</span></span>|
|<span data-ttu-id="fd1db-141">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="fd1db-141">lifetimeInMinutes</span></span>|<span data-ttu-id="fd1db-142">Int32</span><span class="sxs-lookup"><span data-stu-id="fd1db-142">Int32</span></span>|<span data-ttu-id="fd1db-143">Время существования temporaryAccessPass в минутах, начиная с startDateTime.</span><span class="sxs-lookup"><span data-stu-id="fd1db-143">The lifetime of the temporaryAccessPass in minutes starting at startDateTime.</span></span> <span data-ttu-id="fd1db-144">Минимум 10, максимум 43200 (эквивалентно 30 дням).</span><span class="sxs-lookup"><span data-stu-id="fd1db-144">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>|
|<span data-ttu-id="fd1db-145">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="fd1db-145">isUsableOnce</span></span>|<span data-ttu-id="fd1db-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd1db-146">Boolean</span></span>|<span data-ttu-id="fd1db-147">Определяет, ограничен ли проход одновейным использованием.</span><span class="sxs-lookup"><span data-stu-id="fd1db-147">Determines whether the pass is limited to a one time use.</span></span> <span data-ttu-id="fd1db-148">Если этот проход можно использовать один раз; если этот проход можно использовать несколько раз в течение `true` `false` срока действия temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="fd1db-148">If `true`, the pass can be used once; if `false`, the pass can be used multiple times within the temporaryAccessPass lifetime.</span></span>|
|<span data-ttu-id="fd1db-149">isUsable</span><span class="sxs-lookup"><span data-stu-id="fd1db-149">isUsable</span></span>|<span data-ttu-id="fd1db-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd1db-150">Boolean</span></span>|<span data-ttu-id="fd1db-151">Состояние метода проверки подлинности, который указывает, может ли пользователь в настоящее время его указать.</span><span class="sxs-lookup"><span data-stu-id="fd1db-151">The state of the authentication method that indicates whether it's currently usable by the user.</span></span>|
|<span data-ttu-id="fd1db-152">methodUsabilityReason</span><span class="sxs-lookup"><span data-stu-id="fd1db-152">methodUsabilityReason</span></span>|<span data-ttu-id="fd1db-153">String</span><span class="sxs-lookup"><span data-stu-id="fd1db-153">String</span></span>|<span data-ttu-id="fd1db-154">Сведения о состоянии использования (isUsable).</span><span class="sxs-lookup"><span data-stu-id="fd1db-154">Details about usability state (isUsable).</span></span> <span data-ttu-id="fd1db-155">Причины могут быть: `enabledByPolicy` , , , , `disabledByPolicy` `expired` `notYetValid` `oneTimeUsed` .</span><span class="sxs-lookup"><span data-stu-id="fd1db-155">Reasons can include: `enabledByPolicy`, `disabledByPolicy`, `expired`, `notYetValid`, `oneTimeUsed`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="fd1db-156">Связи</span><span class="sxs-lookup"><span data-stu-id="fd1db-156">Relationships</span></span>
<span data-ttu-id="fd1db-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fd1db-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd1db-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="fd1db-158">JSON representation</span></span>
<span data-ttu-id="fd1db-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="fd1db-159">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  "id": "String (identifier)",
  "temporaryAccessPass": "String",
  "createdDateTime": "String (timestamp)",
  "startDateTime": "String (timestamp)",
  "lifetimeInMinutes": "Integer",
  "isUsableOnce": "Boolean",
  "isUsable": "Boolean",
  "methodUsabilityReason": "String"
}
```
