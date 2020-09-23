---
title: Тип ресурса Чатмессажеполицивиолатионполицитип
description: Представляет свойства подсказки политики для объекта Чатмессажеполицивиолатион. Подсказки политики предоставляют отправителю сведения о нарушении политики.
author: laujan
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1ccc3680f5b0365e1f54e9b82743b6906750b272
ms.sourcegitcommit: a3fc420a5639c0f4e89af2b602db17392e176802
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/23/2020
ms.locfileid: "48223959"
---
# <a name="chatmessagepolicytip-resource-type"></a><span data-ttu-id="99df0-104">Тип ресурса Чатмессажеполицитип</span><span class="sxs-lookup"><span data-stu-id="99df0-104">chatMessagePolicyTip resource type</span></span>

<span data-ttu-id="99df0-105">Представляет свойства подсказки политики для объекта [чатмессажеполицивиолатион](chatmessagepolicyviolation.md) .</span><span class="sxs-lookup"><span data-stu-id="99df0-105">Represents the properties of a policy tip on a [chatMessagePolicyViolation](chatmessagepolicyviolation.md) object.</span></span> <span data-ttu-id="99df0-106">Подсказки политики предоставляют отправителю сведения о нарушении политики.</span><span class="sxs-lookup"><span data-stu-id="99df0-106">Policy tips provide the sender with information about the policy violation.</span></span>
<span data-ttu-id="99df0-107">Подсказка политики обычно задается с помощью приложения защиты от потери данных (DLP), которое отслеживает сообщения, содержащие данные, которые не предполагается отправлять пользователям.</span><span class="sxs-lookup"><span data-stu-id="99df0-107">Policy tips are typically set by a data loss prevention (DLP) app which watches for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="99df0-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="99df0-108">Properties</span></span>

| <span data-ttu-id="99df0-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="99df0-109">Property</span></span>   | <span data-ttu-id="99df0-110">Тип</span><span class="sxs-lookup"><span data-stu-id="99df0-110">Type</span></span> |<span data-ttu-id="99df0-111">Описание</span><span class="sxs-lookup"><span data-stu-id="99df0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99df0-112">комплианцеурл</span><span class="sxs-lookup"><span data-stu-id="99df0-112">complianceUrl</span></span>|<span data-ttu-id="99df0-113">string</span><span class="sxs-lookup"><span data-stu-id="99df0-113">string</span></span>|<span data-ttu-id="99df0-114">URL-адрес, который пользователь может посетить для чтения сведений о политиках защиты от потери данных в Организации.</span><span class="sxs-lookup"><span data-stu-id="99df0-114">The URL a user can visit to read about the data loss prevention policies for the organization.</span></span> <span data-ttu-id="99df0-115">(IE, политики о том, что пользователи не должны говорить в беседах)</span><span class="sxs-lookup"><span data-stu-id="99df0-115">(ie, policies about what users shouldn't say in chats)</span></span>|
|<span data-ttu-id="99df0-116">женералтекст</span><span class="sxs-lookup"><span data-stu-id="99df0-116">generalText</span></span>|<span data-ttu-id="99df0-117">string</span><span class="sxs-lookup"><span data-stu-id="99df0-117">string</span></span>|<span data-ttu-id="99df0-118">Пояснительный текст, отображаемый отправителю сообщения.</span><span class="sxs-lookup"><span data-stu-id="99df0-118">Explanatory text shown to the sender of the message.</span></span>|
|<span data-ttu-id="99df0-119">матчедкондитиондескриптионс</span><span class="sxs-lookup"><span data-stu-id="99df0-119">matchedConditionDescriptions</span></span>|<span data-ttu-id="99df0-120">Коллекция строк</span><span class="sxs-lookup"><span data-stu-id="99df0-120">string collection</span></span>|<span data-ttu-id="99df0-121">Список ненужных данных в сообщении, обнаруженном приложением защиты от потери данных.</span><span class="sxs-lookup"><span data-stu-id="99df0-121">The list of improper data in the message that was detected by the data loss prevention app.</span></span> <span data-ttu-id="99df0-122">Каждое приложение DLP определяет собственные условия, например "номер кредитной карты" и "номер социального страхования".</span><span class="sxs-lookup"><span data-stu-id="99df0-122">Each DLP app defines its own conditions, examples include "Credit Card Number" and "Social Security Number".</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99df0-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="99df0-123">JSON representation</span></span>

<span data-ttu-id="99df0-124">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="99df0-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "generalText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"
}-->

```json
{
  "complianceUrl": "string",
  "generalText": "string",
  "matchedConditionDescriptions": ["string 1", "string 2"]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "policy violation policy tip resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
