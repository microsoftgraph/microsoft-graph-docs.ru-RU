---
title: temporaryAccessPassAuthenticationMethod type
description: Представляет временный пропуск доступа, зарегистрированный пользователю.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1bd5bd1ab118d7ec5c7443c47bda1ea614f31bf0
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442812"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a><span data-ttu-id="d4199-103">temporaryAccessPassAuthenticationMethod type</span><span class="sxs-lookup"><span data-stu-id="d4199-103">temporaryAccessPassAuthenticationMethod resource type</span></span>

<span data-ttu-id="d4199-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d4199-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4199-105">Представляет временный пропуск доступа, зарегистрированный пользователю.</span><span class="sxs-lookup"><span data-stu-id="d4199-105">Represents a Temporary Access Pass registered to a user.</span></span> <span data-ttu-id="d4199-106">Временный пропуск доступа — это ограниченный по времени пароль, который служит прочным учетным данным и позволяет использовать учетные данные без паролей.</span><span class="sxs-lookup"><span data-stu-id="d4199-106">A Temporary Access Pass is a time-limited passcode that serves as a strong credential and allows onboarding of passwordless credentials.</span></span>

## <a name="methods"></a><span data-ttu-id="d4199-107">Методы</span><span class="sxs-lookup"><span data-stu-id="d4199-107">Methods</span></span>
|<span data-ttu-id="d4199-108">Метод</span><span class="sxs-lookup"><span data-stu-id="d4199-108">Method</span></span>|<span data-ttu-id="d4199-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="d4199-109">Return type</span></span>|<span data-ttu-id="d4199-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d4199-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4199-111">Список</span><span class="sxs-lookup"><span data-stu-id="d4199-111">List</span></span>](../api/temporaryaccesspassauthenticationmethod-list.md)|<span data-ttu-id="d4199-112">[коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="d4199-112">[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) collection</span></span>|<span data-ttu-id="d4199-113">Извлечение списка временных **объектовAccessPassAuthenticationMethod** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="d4199-113">Retrieve a list of a user's **temporaryAccessPassAuthenticationMethod** objects and their properties.</span></span> <span data-ttu-id="d4199-114">У пользователей может быть только один метод проверки подлинности временных пропусков доступа.</span><span class="sxs-lookup"><span data-stu-id="d4199-114">Users can only have one Temporary Access Pass authentication method.</span></span>|
|[<span data-ttu-id="d4199-115">Создание</span><span class="sxs-lookup"><span data-stu-id="d4199-115">Create</span></span>](../api/temporaryaccesspassauthenticationmethod-post.md)|[<span data-ttu-id="d4199-116">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d4199-116">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="d4199-117">Создайте временный **объектAccessPassAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="d4199-117">Create a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|
|<span data-ttu-id="d4199-118">[получение](../api/temporaryaccesspassauthenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="d4199-118">[Get](../api/temporaryaccesspassauthenticationmethod-get.md)</span></span>|[<span data-ttu-id="d4199-119">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="d4199-119">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="d4199-120">Извлечение свойств объекта **temporaryAccessPassAuthenticationMethod** пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4199-120">Retrieve the properties of the user's **temporaryAccessPassAuthenticationMethod** object.</span></span>||
|<span data-ttu-id="d4199-121">[удаление](../api/temporaryaccesspassauthenticationmethod-delete.md);</span><span class="sxs-lookup"><span data-stu-id="d4199-121">[Delete](../api/temporaryaccesspassauthenticationmethod-delete.md)</span></span>|<span data-ttu-id="d4199-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d4199-122">None</span></span>|<span data-ttu-id="d4199-123">Удаление объекта **temporaryAccessPassAuthenticationMethod** пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4199-123">Delete a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4199-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="d4199-124">Properties</span></span>
|<span data-ttu-id="d4199-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="d4199-125">Property</span></span>|<span data-ttu-id="d4199-126">Тип</span><span class="sxs-lookup"><span data-stu-id="d4199-126">Type</span></span>|<span data-ttu-id="d4199-127">Описание</span><span class="sxs-lookup"><span data-stu-id="d4199-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4199-128">id</span><span class="sxs-lookup"><span data-stu-id="d4199-128">id</span></span>|<span data-ttu-id="d4199-129">String</span><span class="sxs-lookup"><span data-stu-id="d4199-129">String</span></span>|<span data-ttu-id="d4199-130">Идентификатор временного пропуска доступа, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4199-130">The identifier of the Temporary Access Pass registered to this user.</span></span>|
|<span data-ttu-id="d4199-131">temporaryAccessPass</span><span class="sxs-lookup"><span data-stu-id="d4199-131">temporaryAccessPass</span></span>|<span data-ttu-id="d4199-132">String</span><span class="sxs-lookup"><span data-stu-id="d4199-132">String</span></span>|<span data-ttu-id="d4199-133">Для проверки подлинности используется temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="d4199-133">The temporaryAccessPass used to authenticate.</span></span> <span data-ttu-id="d4199-134">Возвращается только при создании нового временногоAccessPass; возвращается как NULL с GET.</span><span class="sxs-lookup"><span data-stu-id="d4199-134">Returned only on creation of a new temporaryAccessPass; returned as NULL with GET.</span></span>|
|<span data-ttu-id="d4199-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4199-135">createdDateTime</span></span>|<span data-ttu-id="d4199-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4199-136">DateTimeOffset</span></span>|<span data-ttu-id="d4199-137">Дата и время создания временногоAccessPass.</span><span class="sxs-lookup"><span data-stu-id="d4199-137">The date and time when the temporaryAccessPass was created.</span></span>|
|<span data-ttu-id="d4199-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="d4199-138">startDateTime</span></span>|<span data-ttu-id="d4199-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4199-139">DateTimeOffset</span></span>|<span data-ttu-id="d4199-140">Дата и время, когда становится доступным для использования temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="d4199-140">The date and time when the temporaryAccessPass becomes available to use.</span></span>|
|<span data-ttu-id="d4199-141">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="d4199-141">lifetimeInMinutes</span></span>|<span data-ttu-id="d4199-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d4199-142">Int32</span></span>|<span data-ttu-id="d4199-143">Срок службы temporaryAccessPass в минутах, начиная с startDateTime.</span><span class="sxs-lookup"><span data-stu-id="d4199-143">The lifetime of the temporaryAccessPass in minutes starting at startDateTime.</span></span> <span data-ttu-id="d4199-144">Минимум 10, максимум 43200 (эквивалент 30 дней).</span><span class="sxs-lookup"><span data-stu-id="d4199-144">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>|
|<span data-ttu-id="d4199-145">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="d4199-145">isUsableOnce</span></span>|<span data-ttu-id="d4199-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4199-146">Boolean</span></span>|<span data-ttu-id="d4199-147">Определяет, ограничен ли пропуск одно время использования.</span><span class="sxs-lookup"><span data-stu-id="d4199-147">Determines whether the pass is limited to a one time use.</span></span> <span data-ttu-id="d4199-148">Если пропуск можно использовать один раз; если пропуск можно использовать несколько раз в течение `true` `false` срока службы temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="d4199-148">If `true`, the pass can be used once; if `false`, the pass can be used multiple times within the temporaryAccessPass lifetime.</span></span>|
|<span data-ttu-id="d4199-149">isUsable</span><span class="sxs-lookup"><span data-stu-id="d4199-149">isUsable</span></span>|<span data-ttu-id="d4199-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4199-150">Boolean</span></span>|<span data-ttu-id="d4199-151">Состояние метода проверки подлинности, которое указывает, является ли он в настоящее время удобным для пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4199-151">The state of the authentication method that indicates whether it's currently usable by the user.</span></span>|
|<span data-ttu-id="d4199-152">methodUsabilityReason</span><span class="sxs-lookup"><span data-stu-id="d4199-152">methodUsabilityReason</span></span>|<span data-ttu-id="d4199-153">String</span><span class="sxs-lookup"><span data-stu-id="d4199-153">String</span></span>|<span data-ttu-id="d4199-154">Сведения о состоянии использования (isUsable).</span><span class="sxs-lookup"><span data-stu-id="d4199-154">Details about usability state (isUsable).</span></span> <span data-ttu-id="d4199-155">Причины могут включать: `enabledByPolicy` `disabledByPolicy` , , , `expired` `notYetValid` `oneTimeUsed` .</span><span class="sxs-lookup"><span data-stu-id="d4199-155">Reasons can include: `enabledByPolicy`, `disabledByPolicy`, `expired`, `notYetValid`, `oneTimeUsed`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="d4199-156">Связи</span><span class="sxs-lookup"><span data-stu-id="d4199-156">Relationships</span></span>
<span data-ttu-id="d4199-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d4199-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4199-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d4199-158">JSON representation</span></span>
<span data-ttu-id="d4199-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d4199-159">The following is a JSON representation of the resource.</span></span>
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
