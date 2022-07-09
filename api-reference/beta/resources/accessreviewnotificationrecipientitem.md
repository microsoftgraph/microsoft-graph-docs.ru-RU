---
title: Тип ресурса accessReviewNotificationRecipientItem
description: Определяет пользователей или группы, которые будут получать уведомления о проверке доступа.
author: zhusijia26
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: a31c9af76dd163e59ac87efed0de53a779534ae3
ms.sourcegitcommit: a08b7dc29c4fd9b5c1c805e47ca824c633f3128f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2022
ms.locfileid: "66697157"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>Тип ресурса accessReviewNotificationRecipientItem

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


Представляет событие Azure AD [проверки доступа](accessreviewsv2-overview.md) для экземпляра проверки. Этот элемент содержит тип шаблона электронной почты и свойства получателя, позволяющие отправлять уведомления определенного типа для данного экземпляра [проверки доступа](accessreviewinstance.md).

## <a name="properties"></a>Свойства

| Свойство                     | Тип     | Описание                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |Строка  | Указывает тип сообщения электронной почты для проверки доступа, которое будет отправлено. Поддерживаемый тип шаблона `CompletedAdditionalRecipients` — отправка получателям уведомлений о завершении проверки.|
| notificationRecipientScope |[accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)  | Определяет получателя уведомления по электронной почте.|

## <a name="relationships"></a>Связи
Отсутствуют.


## <a name="json-representation"></a>Представление JSON

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
