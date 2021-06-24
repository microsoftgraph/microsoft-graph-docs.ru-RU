---
title: тип ресурса serviceUpdateMessage
description: Представляет объявления об изменениях в службе.
author: payiAzure
localization_priority: Normal
ms.prod: service-communications
doc_type: resourcePageType
ms.openlocfilehash: e8bea9b3c44f99d5be0d87b01d47db4505873681
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109226"
---
# <a name="serviceupdatemessage-resource-type"></a><span data-ttu-id="6e134-103">тип ресурса serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="6e134-103">serviceUpdateMessage resource type</span></span>

<span data-ttu-id="6e134-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e134-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6e134-105">Представляет объявления об изменениях в службе.</span><span class="sxs-lookup"><span data-stu-id="6e134-105">Represents the announcements about changes in a service.</span></span>

<span data-ttu-id="6e134-106">Представляет такие объявления, как основные обновления, новые функции в продукте; например, публикация нового Windows.</span><span class="sxs-lookup"><span data-stu-id="6e134-106">Represents announcements such as major updates, new features in a product; for example, the publication of a new Windows feature.</span></span>

<span data-ttu-id="6e134-107">Наследует от [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="6e134-107">Inherits from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>

## <a name="methods"></a><span data-ttu-id="6e134-108">Методы</span><span class="sxs-lookup"><span data-stu-id="6e134-108">Methods</span></span>
|<span data-ttu-id="6e134-109">Метод</span><span class="sxs-lookup"><span data-stu-id="6e134-109">Method</span></span>|<span data-ttu-id="6e134-110">Тип возвращаемых данных</span><span class="sxs-lookup"><span data-stu-id="6e134-110">Return type</span></span>|<span data-ttu-id="6e134-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6e134-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6e134-112">Get serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="6e134-112">Get serviceUpdateMessage</span></span>](../api/serviceupdatemessage-get.md)|[<span data-ttu-id="6e134-113">serviceUpdateMessage</span><span class="sxs-lookup"><span data-stu-id="6e134-113">serviceUpdateMessage</span></span>](../resources/serviceupdatemessage.md)|<span data-ttu-id="6e134-114">Извлечение свойств и связей объекта [serviceUpdateMessage.](../resources/serviceupdatemessage.md)</span><span class="sxs-lookup"><span data-stu-id="6e134-114">Retrieve the properties and relationships of a [serviceUpdateMessage](../resources/serviceupdatemessage.md) object.</span></span> |
|[<span data-ttu-id="6e134-115">markRead</span><span class="sxs-lookup"><span data-stu-id="6e134-115">markRead</span></span>](../api/serviceupdatemessage-markread.md)|<span data-ttu-id="6e134-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e134-116">Boolean</span></span>|<span data-ttu-id="6e134-117">Пометить список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s в качестве чтения для подписанного пользователя. </span><span class="sxs-lookup"><span data-stu-id="6e134-117">Mark a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s as **read** for the signed in user.</span></span>|
|[<span data-ttu-id="6e134-118">markUnread</span><span class="sxs-lookup"><span data-stu-id="6e134-118">markUnread</span></span>](../api/serviceupdatemessage-markunread.md)|<span data-ttu-id="6e134-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e134-119">Boolean</span></span>|<span data-ttu-id="6e134-120">Пометить список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s как непрочитанные для подписанного пользователя. </span><span class="sxs-lookup"><span data-stu-id="6e134-120">Mark a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s as **unread** for the signed in user.</span></span>|
|[<span data-ttu-id="6e134-121">архив</span><span class="sxs-lookup"><span data-stu-id="6e134-121">archive</span></span>](../api/serviceupdatemessage-archive.md)|<span data-ttu-id="6e134-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e134-122">Boolean</span></span>|<span data-ttu-id="6e134-123">Архивировать список [serviceUpdateMessage](../resources/serviceupdatemessage.md)s для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e134-123">Archive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|
|[<span data-ttu-id="6e134-124">unarchive</span><span class="sxs-lookup"><span data-stu-id="6e134-124">unarchive</span></span>](../api/serviceupdatemessage-unarchive.md)|<span data-ttu-id="6e134-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e134-125">Boolean</span></span>|<span data-ttu-id="6e134-126">Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span><span class="sxs-lookup"><span data-stu-id="6e134-126">Unarchive a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|
|[<span data-ttu-id="6e134-127">избранное</span><span class="sxs-lookup"><span data-stu-id="6e134-127">favorite</span></span>](../api/serviceupdatemessage-favorite.md)|<span data-ttu-id="6e134-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e134-128">Boolean</span></span>|<span data-ttu-id="6e134-129">Измените состояние списка [serviceUpdateMessage](../resources/serviceupdatemessage.md)s на избранное для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e134-129">Change the status of a list of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s to favorite for the signed in user.</span></span>|
|[<span data-ttu-id="6e134-130">unfavorite</span><span class="sxs-lookup"><span data-stu-id="6e134-130">unfavorite</span></span>](../api/serviceupdatemessage-unfavorite.md)|<span data-ttu-id="6e134-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e134-131">Boolean</span></span>|<span data-ttu-id="6e134-132">Удалите любимый статус [serviceUpdateMessage](../resources/serviceupdatemessage.md)s для подписанного пользователя.</span><span class="sxs-lookup"><span data-stu-id="6e134-132">Remove the favorite status of [serviceUpdateMessage](../resources/serviceupdatemessage.md)s for the signed in user.</span></span>|

## <a name="properties"></a><span data-ttu-id="6e134-133">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e134-133">Properties</span></span>
|<span data-ttu-id="6e134-134">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e134-134">Property</span></span>|<span data-ttu-id="6e134-135">Тип</span><span class="sxs-lookup"><span data-stu-id="6e134-135">Type</span></span>|<span data-ttu-id="6e134-136">Описание</span><span class="sxs-lookup"><span data-stu-id="6e134-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e134-137">actionRequiredByDateTime</span><span class="sxs-lookup"><span data-stu-id="6e134-137">actionRequiredByDateTime</span></span>|<span data-ttu-id="6e134-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e134-138">DateTimeOffset</span></span>|<span data-ttu-id="6e134-139">Ожидаемый крайний срок действия для сообщения.</span><span class="sxs-lookup"><span data-stu-id="6e134-139">The expected deadline of the action for the message.</span></span>|
|<span data-ttu-id="6e134-140">body</span><span class="sxs-lookup"><span data-stu-id="6e134-140">body</span></span>|[<span data-ttu-id="6e134-141">itemBody</span><span class="sxs-lookup"><span data-stu-id="6e134-141">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="6e134-142">Тип контента и содержимое тела сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-142">The content type and content of the service message body.</span></span>|
|<span data-ttu-id="6e134-143">category</span><span class="sxs-lookup"><span data-stu-id="6e134-143">category</span></span>|<span data-ttu-id="6e134-144">serviceUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="6e134-144">serviceUpdateCategory</span></span>|<span data-ttu-id="6e134-145">Категория сообщений службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-145">The service message category.</span></span> <span data-ttu-id="6e134-146">Возможные значения: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6e134-146">Possible values are: `preventOrFixIssue`, `planForChange`, `stayInformed`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6e134-147">подробности</span><span class="sxs-lookup"><span data-stu-id="6e134-147">details</span></span>|<span data-ttu-id="6e134-148">[Коллекция(keyValuePair)](../resources/keyvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="6e134-148">Collection([keyValuePair](../resources/keyvaluepair.md))</span></span>|<span data-ttu-id="6e134-149">Дополнительные сведения о сообщении службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-149">Additional details about service message.</span></span> <span data-ttu-id="6e134-150">Это свойство не поддерживает фильтры.</span><span class="sxs-lookup"><span data-stu-id="6e134-150">This property doesn't support filters.</span></span> <span data-ttu-id="6e134-151">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="6e134-151">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="6e134-152">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6e134-152">endDateTime</span></span>|<span data-ttu-id="6e134-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e134-153">DateTimeOffset</span></span>|<span data-ttu-id="6e134-154">Конечное время сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-154">The end time of the service message.</span></span> <span data-ttu-id="6e134-155">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="6e134-155">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="6e134-156">id</span><span class="sxs-lookup"><span data-stu-id="6e134-156">id</span></span>|<span data-ttu-id="6e134-157">Строка</span><span class="sxs-lookup"><span data-stu-id="6e134-157">String</span></span>|<span data-ttu-id="6e134-158">Id сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-158">The id of the service message.</span></span> <span data-ttu-id="6e134-159">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="6e134-159">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="6e134-160">isMajorChange</span><span class="sxs-lookup"><span data-stu-id="6e134-160">isMajorChange</span></span>|<span data-ttu-id="6e134-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="6e134-161">Boolean</span></span>|<span data-ttu-id="6e134-162">Указывает, описывает ли сообщение крупное обновление для службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-162">Indicates whether the message describes a major update for the service.</span></span>|
|<span data-ttu-id="6e134-163">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6e134-163">lastModifiedDateTime</span></span>|<span data-ttu-id="6e134-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e134-164">DateTimeOffset</span></span>|<span data-ttu-id="6e134-165">Последнее измененное время сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-165">The last modified time of the service message.</span></span> <span data-ttu-id="6e134-166">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="6e134-166">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="6e134-167">службы</span><span class="sxs-lookup"><span data-stu-id="6e134-167">services</span></span>|<span data-ttu-id="6e134-168">Коллекция (строка)</span><span class="sxs-lookup"><span data-stu-id="6e134-168">Collection(string)</span></span>|<span data-ttu-id="6e134-169">Затронутые службы сообщением службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-169">The affected services by the service message.</span></span>|
|<span data-ttu-id="6e134-170">severity</span><span class="sxs-lookup"><span data-stu-id="6e134-170">severity</span></span>|<span data-ttu-id="6e134-171">serviceUpdateSeverity</span><span class="sxs-lookup"><span data-stu-id="6e134-171">serviceUpdateSeverity</span></span>|<span data-ttu-id="6e134-172">Серьезность сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-172">The severity of the service message.</span></span> <span data-ttu-id="6e134-173">Возможные значения: `normal`, `high`, `critical`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="6e134-173">Possible values are: `normal`, `high`, `critical`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="6e134-174">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6e134-174">startDateTime</span></span>|<span data-ttu-id="6e134-175">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6e134-175">DateTimeOffset</span></span>|<span data-ttu-id="6e134-176">Время начала сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-176">The start time of the service message.</span></span> <span data-ttu-id="6e134-177">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="6e134-177">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="6e134-178">tags</span><span class="sxs-lookup"><span data-stu-id="6e134-178">tags</span></span>|<span data-ttu-id="6e134-179">Коллекция (строка)</span><span class="sxs-lookup"><span data-stu-id="6e134-179">Collection(string)</span></span>|<span data-ttu-id="6e134-180">Коллекция тегов для сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-180">A collection of tags for the service message.</span></span>|
|<span data-ttu-id="6e134-181">title</span><span class="sxs-lookup"><span data-stu-id="6e134-181">title</span></span>|<span data-ttu-id="6e134-182">Строка</span><span class="sxs-lookup"><span data-stu-id="6e134-182">String</span></span>|<span data-ttu-id="6e134-183">Название сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-183">The title of the service message.</span></span> <span data-ttu-id="6e134-184">Наследуется [от serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span><span class="sxs-lookup"><span data-stu-id="6e134-184">Inherited from [serviceAnnouncementBase](../resources/serviceannouncementbase.md).</span></span>|
|<span data-ttu-id="6e134-185">viewPoint</span><span class="sxs-lookup"><span data-stu-id="6e134-185">viewPoint</span></span>|[<span data-ttu-id="6e134-186">serviceUpdateMessageViewpoint</span><span class="sxs-lookup"><span data-stu-id="6e134-186">serviceUpdateMessageViewpoint</span></span>](../resources/serviceupdatemessageviewpoint.md)|<span data-ttu-id="6e134-187">Представляет данные точек представления пользователей сообщения службы.</span><span class="sxs-lookup"><span data-stu-id="6e134-187">Represents user view points data of the service message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e134-188">Отношения</span><span class="sxs-lookup"><span data-stu-id="6e134-188">Relationships</span></span>
<span data-ttu-id="6e134-189">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6e134-189">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e134-190">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="6e134-190">JSON representation</span></span>
<span data-ttu-id="6e134-191">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e134-191">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.serviceUpdateMessage",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.serviceUpdateMessage",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "title": "String",
  "details": [
    {
      "@odata.type": "microsoft.graph.keyValuePair"
    }
  ],
  "id": "String (identifier)",
  "body": {
    "@odata.type": "microsoft.graph.itemBody"
  },
  "category": "String",
  "severity": "String",
  "tags": [
    "String"
  ],
  "isMajorChange": "Boolean",
  "actionRequiredByDateTime": "String (timestamp)",
  "services": [
    "String"
  ],
  "viewPoint": {
    "@odata.type": "microsoft.graph.serviceUpdateMessageViewpoint"
  }
}
```

