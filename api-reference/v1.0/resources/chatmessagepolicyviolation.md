---
title: тип ресурса chatMessagePolicyViolation
description: Представляет нарушение политики в сообщении чата. Нарушения политики обычно устанавливаются приложением для предотвращения потери данных (DLP).
author: RamjotSingh
doc_type: resourcePageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 46d839c6365c148777a280d7af8a36f3bf58ccd1
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582755"
---
# <a name="chatmessagepolicyviolation-resource-type"></a><span data-ttu-id="6fd6e-104">тип ресурса chatMessagePolicyViolation</span><span class="sxs-lookup"><span data-stu-id="6fd6e-104">chatMessagePolicyViolation resource type</span></span>

<span data-ttu-id="6fd6e-105">Представляет нарушение политики в сообщении чата.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-105">Represents a policy violation on a chat message.</span></span> <span data-ttu-id="6fd6e-106">Нарушения политики обычно устанавливаются приложением для предотвращения потери данных (DLP).</span><span class="sxs-lookup"><span data-stu-id="6fd6e-106">Policy violations are typically set by a data loss prevention (DLP) application.</span></span> <span data-ttu-id="6fd6e-107">Приложения DLP отслеживают чаты для сообщений, содержащих данные, которые не должны отправляться пользователями.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-107">DLP applications monitor chats for messages that contain data that users aren't supposed to send.</span></span>

## <a name="properties"></a><span data-ttu-id="6fd6e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6fd6e-108">Properties</span></span>

| <span data-ttu-id="6fd6e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6fd6e-109">Property</span></span>   | <span data-ttu-id="6fd6e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6fd6e-110">Type</span></span> |<span data-ttu-id="6fd6e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6fd6e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6fd6e-112">dlpAction</span><span class="sxs-lookup"><span data-stu-id="6fd6e-112">dlpAction</span></span>|<span data-ttu-id="6fd6e-113">**chatMessagePolicyViolationDlpActionType**</span><span class="sxs-lookup"><span data-stu-id="6fd6e-113">**chatMessagePolicyViolationDlpActionType**</span></span>|<span data-ttu-id="6fd6e-114">Действия, принятые поставщиком DLP в сообщении с конфиденциальным контентом.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-114">The action taken by the DLP provider on the message with sensitive content.</span></span> <span data-ttu-id="6fd6e-115">Поддерживаемые значения:</span><span class="sxs-lookup"><span data-stu-id="6fd6e-115">Supported values are:</span></span> <li><span data-ttu-id="6fd6e-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6fd6e-116">None</span></span></li><li><span data-ttu-id="6fd6e-117">NotifySender . Информируйте отправитель о нарушении, но позвольте читателям прочитать сообщение.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-117">NotifySender -- Inform the sender of the violation but allow readers to read the message.</span></span></li><li><span data-ttu-id="6fd6e-118">BlockAccess . Блокировать чтение сообщения читателями.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-118">BlockAccess -- Block readers from reading the message.</span></span></li><li><span data-ttu-id="6fd6e-119">BlockAccessExternal . Блокировать чтение сообщения пользователями за пределами организации, позволяя пользователям в организации читать сообщение.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-119">BlockAccessExternal -- Block users outside the organization from reading the message, while allowing users within the organization to read the message.</span></span></li>|
|<span data-ttu-id="6fd6e-120">justificationText</span><span class="sxs-lookup"><span data-stu-id="6fd6e-120">justificationText</span></span>|<span data-ttu-id="6fd6e-121">string</span><span class="sxs-lookup"><span data-stu-id="6fd6e-121">string</span></span>|<span data-ttu-id="6fd6e-122">Текст обоснования, предоставляемый отправитель сообщения при переопределения нарушения политики.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-122">Justification text provided by the sender of the message when overriding a policy violation.</span></span>|
|<span data-ttu-id="6fd6e-123">policyTip</span><span class="sxs-lookup"><span data-stu-id="6fd6e-123">policyTip</span></span>|[<span data-ttu-id="6fd6e-124">chatMessagePolicyViolationPolicyTip</span><span class="sxs-lookup"><span data-stu-id="6fd6e-124">chatMessagePolicyViolationPolicyTip</span></span>](chatmessagepolicyviolationpolicytip.md)|<span data-ttu-id="6fd6e-125">Сведения для отображения отправилю сообщения о том, почему сообщение было помечено как нарушение.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-125">Information to display to the message sender about why the message was flagged as a violation.</span></span> |
|<span data-ttu-id="6fd6e-126">userAction</span><span class="sxs-lookup"><span data-stu-id="6fd6e-126">userAction</span></span>|<span data-ttu-id="6fd6e-127">**chatMessagePolicyViolationUserActionType**</span><span class="sxs-lookup"><span data-stu-id="6fd6e-127">**chatMessagePolicyViolationUserActionType**</span></span>|<span data-ttu-id="6fd6e-128">Указывает действие пользователя на сообщение, заблокированное поставщиком DLP.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-128">Indicates the action taken by the user on a message blocked by the DLP provider.</span></span> <span data-ttu-id="6fd6e-129">Поддерживаемые значения:</span><span class="sxs-lookup"><span data-stu-id="6fd6e-129">Supported values are:</span></span> <li><span data-ttu-id="6fd6e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="6fd6e-130">None</span></span></li><li><span data-ttu-id="6fd6e-131">Override</span><span class="sxs-lookup"><span data-stu-id="6fd6e-131">Override</span></span></li><li><span data-ttu-id="6fd6e-132">ReportFalsePositive</span><span class="sxs-lookup"><span data-stu-id="6fd6e-132">ReportFalsePositive</span></span></li><span data-ttu-id="6fd6e-133">Когда поставщик DLP обновляет сообщение для блокировки конфиденциального контента, userAction не требуется.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-133">When the DLP provider is updating the message for blocking sensitive content, userAction is not required.</span></span>|
|<span data-ttu-id="6fd6e-134">verdictDetails</span><span class="sxs-lookup"><span data-stu-id="6fd6e-134">verdictDetails</span></span>|<span data-ttu-id="6fd6e-135">**chatMessagePolicyViolationVerdictDetailsType**</span><span class="sxs-lookup"><span data-stu-id="6fd6e-135">**chatMessagePolicyViolationVerdictDetailsType**</span></span>|<span data-ttu-id="6fd6e-136">Указывает, какие действия может принять отправитель в ответ на нарушение политики.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-136">Indicates what actions the sender may take in response to the policy violation.</span></span> <span data-ttu-id="6fd6e-137">Поддерживаемые значения:</span><span class="sxs-lookup"><span data-stu-id="6fd6e-137">Supported values are:</span></span> <li><span data-ttu-id="6fd6e-138">Нет</span><span class="sxs-lookup"><span data-stu-id="6fd6e-138">None</span></span></li><li><span data-ttu-id="6fd6e-139">AllowFalsePositiveOverride — позволяет отправителю объявить политикуViolation ошибкой в приложении DLP и его правилах, а также разрешить читателям снова видеть сообщение, если dlpAction его спрятал.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-139">AllowFalsePositiveOverride -- Allows the sender to declare the policyViolation to be an error in the DLP app and its rules, and allow readers to see the message again if the dlpAction had hidden it.</span></span></li><li><span data-ttu-id="6fd6e-140">AllowOverrideWithoutJustification — позволяет отправителю перезахотрить нарушение DLP и разрешить читателям видеть сообщение снова, если dlpAction спрятал его, не ая при этом объяснений.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-140">AllowOverrideWithoutJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, without needing to provide an explanation for doing so.</span></span> </li><li><span data-ttu-id="6fd6e-141">AllowOverrideWithJustification — позволяет отправителю перезахотрить нарушение DLP и разрешить читателям снова видеть сообщение, если dlpAction спрятал его, после предоставления объяснений для этого.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-141">AllowOverrideWithJustification -- Allows the sender to overriide the DLP violation and allow readers to see the message again if the dlpAction had hidden it, after providing an explanation for doing so.</span></span></li><span data-ttu-id="6fd6e-142">AllowOverrideWithoutJustification и AllowOverrideWithJustification являются взаимоисключающими.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-142">AllowOverrideWithoutJustification and AllowOverrideWithJustification are mutually exclusive.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6fd6e-143">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6fd6e-143">JSON representation</span></span>

<span data-ttu-id="6fd6e-144">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6fd6e-144">The following is a JSON representation of the resource.</span></span>

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
