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
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>accessReviewNotificationRecipientItem resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


Представляет событие уведомления об уведомлении о просмотре доступа Azure [AD](accessreviewsv2-root.md) в экземпляре проверки. Этот элемент содержит тип шаблона электронной почты и свойства получателей, чтобы включить отправку определенных типов уведомлений для данного экземпляра [обзора доступа.](accessreviewinstance.md)

## <a name="properties"></a>Свойства

| Свойство                     | Тип     | Описание                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |String  | Указывает тип отправки электронной почты для проверки доступа. Поддерживаемый тип шаблона — это отправка получателям уведомлений о `CompletedAdditionalRecipients` завершении проверки.|
| notificationRecipientScope |[accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)  | Определяет получателя сообщения уведомления.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

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
