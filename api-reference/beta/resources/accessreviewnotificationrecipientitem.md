---
title: accessReviewNotificationRecipientItem resource type
description: Определяет пользователей или группы, которые будут получать уведомления о просмотре доступа к уведомлениям.
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 3d6ed767f1350f3e4a43a1b31363920ffb58a9b5
ms.sourcegitcommit: 7abb0672a38a6d9b11a2e0d2cc221222cb8358bb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2021
ms.locfileid: "52896744"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a><span data-ttu-id="71df4-103">accessReviewNotificationRecipientItem resource type</span><span class="sxs-lookup"><span data-stu-id="71df4-103">accessReviewNotificationRecipientItem resource type</span></span>

<span data-ttu-id="71df4-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71df4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


<span data-ttu-id="71df4-105">Представляет событие уведомления об уведомлении о просмотре доступа Azure [AD](accessreviewsv2-root.md) в экземпляре проверки.</span><span class="sxs-lookup"><span data-stu-id="71df4-105">Represents an Azure AD [access review](accessreviewsv2-root.md) notification event on an instance of a review.</span></span> <span data-ttu-id="71df4-106">Этот элемент содержит тип шаблона электронной почты и свойства получателей, чтобы включить отправку определенных типов уведомлений для данного экземпляра [обзора доступа.](accessreviewinstance.md)</span><span class="sxs-lookup"><span data-stu-id="71df4-106">This item contains an email template type and recipient properties to enable sending certain type of notifications for a given [access review instance](accessreviewinstance.md).</span></span>

## <a name="properties"></a><span data-ttu-id="71df4-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="71df4-107">Properties</span></span>

| <span data-ttu-id="71df4-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="71df4-108">Property</span></span>                     | <span data-ttu-id="71df4-109">Тип</span><span class="sxs-lookup"><span data-stu-id="71df4-109">Type</span></span>     | <span data-ttu-id="71df4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="71df4-110">Description</span></span>                          |
| :--------------------------- | :------  | :----------                          |
| <span data-ttu-id="71df4-111">notificationTemplateType</span><span class="sxs-lookup"><span data-stu-id="71df4-111">notificationTemplateType</span></span>  |<span data-ttu-id="71df4-112">String</span><span class="sxs-lookup"><span data-stu-id="71df4-112">String</span></span>  | <span data-ttu-id="71df4-113">Указывает тип отправки электронной почты для проверки доступа.</span><span class="sxs-lookup"><span data-stu-id="71df4-113">Indicates the type of access review email to be sent.</span></span> <span data-ttu-id="71df4-114">Поддерживаемый тип шаблона — это отправка получателям уведомлений о `CompletedAdditionalRecipients` завершении проверки.</span><span class="sxs-lookup"><span data-stu-id="71df4-114">Supported template type is `CompletedAdditionalRecipients` which sends review completion notifications to the recipients.</span></span>|
| <span data-ttu-id="71df4-115">notificationRecipientScope</span><span class="sxs-lookup"><span data-stu-id="71df4-115">notificationRecipientScope</span></span> |[<span data-ttu-id="71df4-116">accessReviewNotificationRecipientScope</span><span class="sxs-lookup"><span data-stu-id="71df4-116">accessReviewNotificationRecipientScope</span></span>](../resources/accessreviewnotificationrecipientscope.md)  | <span data-ttu-id="71df4-117">Определяет получателя сообщения уведомления.</span><span class="sxs-lookup"><span data-stu-id="71df4-117">Determines the recipient of the notification email.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71df4-118">Связи</span><span class="sxs-lookup"><span data-stu-id="71df4-118">Relationships</span></span>
<span data-ttu-id="71df4-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="71df4-119">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="71df4-120">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="71df4-120">JSON representation</span></span>

<span data-ttu-id="71df4-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="71df4-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessReviewNotificationRecipientItem",
  "openType": true
}
-->

```json
{
  "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientItem",
  "notificationRecipientScope": {
      "@odata.type":"#microsoft.graph.accessReviewNotificationRecipientQueryScope"                
    },
  "notificationTemplateType": "String"
}
```
