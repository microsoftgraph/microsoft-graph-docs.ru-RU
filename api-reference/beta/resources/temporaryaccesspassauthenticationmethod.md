---
title: temporaryAccessPassAuthenticationMethod type
description: Представляет временный пропуск доступа, зарегистрированный пользователю.
author: inbarckms
ms.author: inbarc
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 8c118978f9e7c8a7c3aa127ba12aba48f2cfe362
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760962"
---
# <a name="temporaryaccesspassauthenticationmethod-resource-type"></a><span data-ttu-id="c3857-103">temporaryAccessPassAuthenticationMethod type</span><span class="sxs-lookup"><span data-stu-id="c3857-103">temporaryAccessPassAuthenticationMethod resource type</span></span>

<span data-ttu-id="c3857-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3857-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3857-105">Представляет временный пропуск доступа, зарегистрированный пользователю.</span><span class="sxs-lookup"><span data-stu-id="c3857-105">Represents a Temporary Access Pass registered to a user.</span></span> <span data-ttu-id="c3857-106">Временный пропуск доступа — это ограниченный по времени пароль, который служит прочным учетным данным и позволяет использовать учетные данные без паролей.</span><span class="sxs-lookup"><span data-stu-id="c3857-106">A Temporary Access Pass is a time-limited passcode that serves as a strong credential and allows onboarding of passwordless credentials.</span></span>

## <a name="methods"></a><span data-ttu-id="c3857-107">Методы</span><span class="sxs-lookup"><span data-stu-id="c3857-107">Methods</span></span>
|<span data-ttu-id="c3857-108">Метод</span><span class="sxs-lookup"><span data-stu-id="c3857-108">Method</span></span>|<span data-ttu-id="c3857-109">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="c3857-109">Return type</span></span>|<span data-ttu-id="c3857-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c3857-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3857-111">Перечисление</span><span class="sxs-lookup"><span data-stu-id="c3857-111">List</span></span>](../api/temporaryaccesspassauthenticationmethod-list.md)|<span data-ttu-id="c3857-112">[коллекция temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="c3857-112">[temporaryAccessPassAuthenticationMethod](../resources/temporaryaccesspassauthenticationmethod.md) collection</span></span>|<span data-ttu-id="c3857-113">Извлечение списка временных **объектовAccessPassAuthenticationMethod** и их свойств.</span><span class="sxs-lookup"><span data-stu-id="c3857-113">Retrieve a list of a user's **temporaryAccessPassAuthenticationMethod** objects and their properties.</span></span> <span data-ttu-id="c3857-114">У пользователей может быть только один метод проверки подлинности временных пропусков доступа.</span><span class="sxs-lookup"><span data-stu-id="c3857-114">Users can only have one Temporary Access Pass authentication method.</span></span>|
|[<span data-ttu-id="c3857-115">Создание</span><span class="sxs-lookup"><span data-stu-id="c3857-115">Create</span></span>](../api/temporaryaccesspassauthenticationmethod-post.md)|[<span data-ttu-id="c3857-116">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c3857-116">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="c3857-117">Создайте временный **объектAccessPassAuthenticationMethod.**</span><span class="sxs-lookup"><span data-stu-id="c3857-117">Create a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|
|<span data-ttu-id="c3857-118">[Получение](../api/temporaryaccesspassauthenticationmethod-get.md);</span><span class="sxs-lookup"><span data-stu-id="c3857-118">[Get](../api/temporaryaccesspassauthenticationmethod-get.md)</span></span>|[<span data-ttu-id="c3857-119">temporaryAccessPassAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="c3857-119">temporaryAccessPassAuthenticationMethod</span></span>](../resources/temporaryaccesspassauthenticationmethod.md)|<span data-ttu-id="c3857-120">Извлечение свойств объекта **temporaryAccessPassAuthenticationMethod** пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3857-120">Retrieve the properties of the user's **temporaryAccessPassAuthenticationMethod** object.</span></span>||
|[<span data-ttu-id="c3857-121">Удаление</span><span class="sxs-lookup"><span data-stu-id="c3857-121">Delete</span></span>](../api/temporaryaccesspassauthenticationmethod-delete.md)|<span data-ttu-id="c3857-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c3857-122">None</span></span>|<span data-ttu-id="c3857-123">Удаление объекта **temporaryAccessPassAuthenticationMethod** пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3857-123">Delete a user's **temporaryAccessPassAuthenticationMethod** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3857-124">Свойства</span><span class="sxs-lookup"><span data-stu-id="c3857-124">Properties</span></span>
|<span data-ttu-id="c3857-125">Свойство</span><span class="sxs-lookup"><span data-stu-id="c3857-125">Property</span></span>|<span data-ttu-id="c3857-126">Тип</span><span class="sxs-lookup"><span data-stu-id="c3857-126">Type</span></span>|<span data-ttu-id="c3857-127">Описание</span><span class="sxs-lookup"><span data-stu-id="c3857-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3857-128">id</span><span class="sxs-lookup"><span data-stu-id="c3857-128">id</span></span>|<span data-ttu-id="c3857-129">String</span><span class="sxs-lookup"><span data-stu-id="c3857-129">String</span></span>|<span data-ttu-id="c3857-130">Идентификатор временного пропуска доступа, зарегистрированного для этого пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3857-130">The identifier of the Temporary Access Pass registered to this user.</span></span>|
|<span data-ttu-id="c3857-131">temporaryAccessPass</span><span class="sxs-lookup"><span data-stu-id="c3857-131">temporaryAccessPass</span></span>|<span data-ttu-id="c3857-132">String</span><span class="sxs-lookup"><span data-stu-id="c3857-132">String</span></span>|<span data-ttu-id="c3857-133">Для проверки подлинности используется temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="c3857-133">The temporaryAccessPass used to authenticate.</span></span> <span data-ttu-id="c3857-134">Возвращается только при создании нового временногоAccessPass; возвращается как NULL с GET.</span><span class="sxs-lookup"><span data-stu-id="c3857-134">Returned only on creation of a new temporaryAccessPass; returned as NULL with GET.</span></span>|
|<span data-ttu-id="c3857-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c3857-135">createdDateTime</span></span>|<span data-ttu-id="c3857-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3857-136">DateTimeOffset</span></span>|<span data-ttu-id="c3857-137">Дата и время создания временногоAccessPass.</span><span class="sxs-lookup"><span data-stu-id="c3857-137">The date and time when the temporaryAccessPass was created.</span></span>|
|<span data-ttu-id="c3857-138">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c3857-138">startDateTime</span></span>|<span data-ttu-id="c3857-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3857-139">DateTimeOffset</span></span>|<span data-ttu-id="c3857-140">Дата и время, когда становится доступным для использования temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="c3857-140">The date and time when the temporaryAccessPass becomes available to use.</span></span>|
|<span data-ttu-id="c3857-141">lifetimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="c3857-141">lifetimeInMinutes</span></span>|<span data-ttu-id="c3857-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c3857-142">Int32</span></span>|<span data-ttu-id="c3857-143">Срок службы temporaryAccessPass в минутах, начиная с startDateTime.</span><span class="sxs-lookup"><span data-stu-id="c3857-143">The lifetime of the temporaryAccessPass in minutes starting at startDateTime.</span></span> <span data-ttu-id="c3857-144">Минимум 10, максимум 43200 (эквивалент 30 дней).</span><span class="sxs-lookup"><span data-stu-id="c3857-144">Minimum 10, Maximum 43200 (equivalent to 30 days).</span></span>|
|<span data-ttu-id="c3857-145">isUsableOnce</span><span class="sxs-lookup"><span data-stu-id="c3857-145">isUsableOnce</span></span>|<span data-ttu-id="c3857-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3857-146">Boolean</span></span>|<span data-ttu-id="c3857-147">Определяет, ограничен ли пропуск одно время использования.</span><span class="sxs-lookup"><span data-stu-id="c3857-147">Determines whether the pass is limited to a one time use.</span></span> <span data-ttu-id="c3857-148">Если пропуск можно использовать один раз; если пропуск можно использовать несколько раз в течение `true` `false` срока службы temporaryAccessPass.</span><span class="sxs-lookup"><span data-stu-id="c3857-148">If `true`, the pass can be used once; if `false`, the pass can be used multiple times within the temporaryAccessPass lifetime.</span></span>|
|<span data-ttu-id="c3857-149">isUsable</span><span class="sxs-lookup"><span data-stu-id="c3857-149">isUsable</span></span>|<span data-ttu-id="c3857-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3857-150">Boolean</span></span>|<span data-ttu-id="c3857-151">Состояние метода проверки подлинности, которое указывает, является ли он в настоящее время удобным для пользователя.</span><span class="sxs-lookup"><span data-stu-id="c3857-151">The state of the authentication method that indicates whether it's currently usable by the user.</span></span>|
|<span data-ttu-id="c3857-152">methodUsabilityReason</span><span class="sxs-lookup"><span data-stu-id="c3857-152">methodUsabilityReason</span></span>|<span data-ttu-id="c3857-153">String</span><span class="sxs-lookup"><span data-stu-id="c3857-153">String</span></span>|<span data-ttu-id="c3857-154">Сведения о состоянии использования (isUsable).</span><span class="sxs-lookup"><span data-stu-id="c3857-154">Details about usability state (isUsable).</span></span> <span data-ttu-id="c3857-155">Причины могут включать: `enabledByPolicy` `disabledByPolicy` , , , `expired` `notYetValid` `oneTimeUsed` .</span><span class="sxs-lookup"><span data-stu-id="c3857-155">Reasons can include: `enabledByPolicy`, `disabledByPolicy`, `expired`, `notYetValid`, `oneTimeUsed`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="c3857-156">Отношения</span><span class="sxs-lookup"><span data-stu-id="c3857-156">Relationships</span></span>
<span data-ttu-id="c3857-157">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c3857-157">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3857-158">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c3857-158">JSON representation</span></span>
<span data-ttu-id="c3857-159">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c3857-159">The following is a JSON representation of the resource.</span></span>
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
