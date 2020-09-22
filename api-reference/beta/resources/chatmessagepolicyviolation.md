---
title: Тип ресурса Чатмессажеполицивиолатион
description: Представляет нарушение политики в сообщении чата. Нарушения политики обычно задаются с помощью приложения предотвращения потери данных (DLP).
author: clearab
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 458e6440806ac57248bb87c6313d78b4845d647f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "48082107"
---
# <a name="chatmessagepolicyviolation-resource-type"></a><span data-ttu-id="e599f-104">Тип ресурса Чатмессажеполицивиолатион</span><span class="sxs-lookup"><span data-stu-id="e599f-104">chatMessagePolicyViolation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e599f-105">Представляет нарушение политики в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="e599f-105">Represents a policy violation on a chat message.</span></span> <span data-ttu-id="e599f-106">Нарушения политики обычно задаются с помощью приложения предотвращения потери данных (DLP).</span><span class="sxs-lookup"><span data-stu-id="e599f-106">Policy violations are typically set by a data loss prevention (DLP) application.</span></span> <span data-ttu-id="e599f-107">Приложения DLP отслеживают сеансы обмена сообщениями, которые содержат данные, которые не предполагается отправлять пользователям.</span><span class="sxs-lookup"><span data-stu-id="e599f-107">DLP applications monitor chats for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="e599f-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e599f-108">Properties</span></span>

| <span data-ttu-id="e599f-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e599f-109">Property</span></span>   | <span data-ttu-id="e599f-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e599f-110">Type</span></span> |<span data-ttu-id="e599f-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e599f-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e599f-112">длпактион</span><span class="sxs-lookup"><span data-stu-id="e599f-112">dlpAction</span></span>|<span data-ttu-id="e599f-113">**чатмессажеполицивиолатиондлпактионтипе**</span><span class="sxs-lookup"><span data-stu-id="e599f-113">**chatMessagePolicyViolationDlpActionType**</span></span>|<span data-ttu-id="e599f-114">Действие, выполняемое поставщиком DLP для сообщения с конфиденциальным содержимым.</span><span class="sxs-lookup"><span data-stu-id="e599f-114">The action taken by the DLP provider on the message with sensitive content.</span></span> <span data-ttu-id="e599f-115">Поддерживаемые значения:</span><span class="sxs-lookup"><span data-stu-id="e599f-115">Supported values are:</span></span> <li><span data-ttu-id="e599f-116">Нет</span><span class="sxs-lookup"><span data-stu-id="e599f-116">None</span></span></li><li><span data-ttu-id="e599f-117">NotifySender — уведомить отправителя о нарушении, но позволить читателям читать сообщение.</span><span class="sxs-lookup"><span data-stu-id="e599f-117">NotifySender -- Inform the sender of the violation but allow readers to read the message.</span></span></li><li><span data-ttu-id="e599f-118">Блоккакцесс запрещает читателям читать сообщение.</span><span class="sxs-lookup"><span data-stu-id="e599f-118">BlockAccess -- Block readers from reading the message.</span></span></li><li><span data-ttu-id="e599f-119">Блоккакцессекстернал — блокировать чтение сообщения пользователями за пределами Организации, в то же время позволяя пользователям в Организации читать сообщение.</span><span class="sxs-lookup"><span data-stu-id="e599f-119">BlockAccessExternal -- Block users outside the organization from reading the message, while allowing users within the organization to read the message.</span></span></li>|
|<span data-ttu-id="e599f-120">жустификатионтекст</span><span class="sxs-lookup"><span data-stu-id="e599f-120">justificationText</span></span>|<span data-ttu-id="e599f-121">string</span><span class="sxs-lookup"><span data-stu-id="e599f-121">string</span></span>|<span data-ttu-id="e599f-122">Текст обоснования, предоставленный отправителем сообщения при переопределении нарушения политики.</span><span class="sxs-lookup"><span data-stu-id="e599f-122">Justification text provided by the sender of the message when overriding a policy violation.</span></span>|
|<span data-ttu-id="e599f-123">полицитип</span><span class="sxs-lookup"><span data-stu-id="e599f-123">policyTip</span></span>|[<span data-ttu-id="e599f-124">чатмессажеполицивиолатионполицитип</span><span class="sxs-lookup"><span data-stu-id="e599f-124">chatMessagePolicyViolationPolicyTip</span></span>](chatmessagepolicyviolationpolicytip.md)|<span data-ttu-id="e599f-125">Сведения, которые должны отображаться у отправителя сообщения о причинах пометки сообщения как нарушения.</span><span class="sxs-lookup"><span data-stu-id="e599f-125">Information to display to the message sender about why the message was flagged as a violation.</span></span> |
|<span data-ttu-id="e599f-126">усерактион</span><span class="sxs-lookup"><span data-stu-id="e599f-126">userAction</span></span>|<span data-ttu-id="e599f-127">**чатмессажеполицивиолатионусерактионтипе**</span><span class="sxs-lookup"><span data-stu-id="e599f-127">**chatMessagePolicyViolationUserActionType**</span></span>|<span data-ttu-id="e599f-128">Указывает действие, выполняемое пользователем для сообщения, заблокированного поставщиком DLP.</span><span class="sxs-lookup"><span data-stu-id="e599f-128">Indicates the action taken by the user on a message blocked by the DLP provider.</span></span> <span data-ttu-id="e599f-129">Поддерживаемые значения:</span><span class="sxs-lookup"><span data-stu-id="e599f-129">Supported values are:</span></span> <li><span data-ttu-id="e599f-130">Нет</span><span class="sxs-lookup"><span data-stu-id="e599f-130">None</span></span></li><li><span data-ttu-id="e599f-131">Override</span><span class="sxs-lookup"><span data-stu-id="e599f-131">Override</span></span></li><li><span data-ttu-id="e599f-132">репортфалсепоситиве</span><span class="sxs-lookup"><span data-stu-id="e599f-132">ReportFalsePositive</span></span></li><span data-ttu-id="e599f-133">Когда поставщик DLP обновляет сообщение для блокирования конфиденциального содержимого, Усерактион не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e599f-133">When the DLP provider is updating the message for blocking sensitive content, userAction is not required.</span></span>|
|<span data-ttu-id="e599f-134">вердиктдетаилс</span><span class="sxs-lookup"><span data-stu-id="e599f-134">verdictDetails</span></span>|<span data-ttu-id="e599f-135">**чатмессажеполицивиолатионвердиктдетаилстипе**</span><span class="sxs-lookup"><span data-stu-id="e599f-135">**chatMessagePolicyViolationVerdictDetailsType**</span></span>|<span data-ttu-id="e599f-136">Указывает, какие действия может предпринять отправитель в ответ на нарушение политики.</span><span class="sxs-lookup"><span data-stu-id="e599f-136">Indicates what actions the sender may take in response to the policy violation.</span></span> <span data-ttu-id="e599f-137">Поддерживаемые значения:</span><span class="sxs-lookup"><span data-stu-id="e599f-137">Supported values are:</span></span> <li><span data-ttu-id="e599f-138">Нет</span><span class="sxs-lookup"><span data-stu-id="e599f-138">None</span></span></li><li><span data-ttu-id="e599f-139">Алловфалсепоситивеоверриде — позволяет отправителю объявить сообщение об ошибке в приложении DLP и его правилах и позволить читателям снова видеть сообщение, если оно было скрыто в Длпактион.</span><span class="sxs-lookup"><span data-stu-id="e599f-139">AllowFalsePositiveOverride -- Allows the sender to declare the policyViolation to be an error in the DLP app and its rules, and allow readers to see the message again if the dlpAction had hidden it.</span></span></li><li><span data-ttu-id="e599f-140">Аллововерридевисаутжустификатион — позволяет отправителю оверрииде нарушение защиты от потери данных и позволить читателям снова видеть сообщение, если оно было скрыто в Длпактион, без необходимости предоставлять объяснение для этого.</span><span class="sxs-lookup"><span data-stu-id="e599f-140">AllowOverrideWithoutJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, without needing to provide an explanation for doing so.</span></span> </li><li><span data-ttu-id="e599f-141">Аллововерридевисжустификатион — позволяет отправителю оверрииде нарушение защиты от потери данных и позволить читателям снова видеть сообщение, если оно было скрыто в Длпактион, после предоставления объяснения для этого.</span><span class="sxs-lookup"><span data-stu-id="e599f-141">AllowOverrideWithJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, after providing an explanation for doing so.</span></span></li><span data-ttu-id="e599f-142">Аллововерридевисаутжустификатион и Аллововерридевисжустификатион являются взаимоисключающими.</span><span class="sxs-lookup"><span data-stu-id="e599f-142">AllowOverrideWithoutJustification and AllowOverrideWithJustification are mutually exclusive.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="e599f-143">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="e599f-143">JSON representation</span></span>

<span data-ttu-id="e599f-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e599f-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "userAction",
    "justificationText"
  ],
  "@odata.type": "microsoft.graph.chatMessagePolicyViolation"
}-->

```json
{
  "dlpAction": "string",
  "justificationText": "string",
  "policyTip": {"@odata.type": "microsoft.graph.chatMessagePolicyViolationPolicyTip"},
  "userAction": "string",
  "verdictDetails": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "chat message policy violation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
