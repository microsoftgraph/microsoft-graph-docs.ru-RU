---
title: accessReviewNotificationRecipientItem resource type
description: Определяет пользователей или группы, которые будут получать уведомления о просмотре доступа к уведомлениям.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 00904cf1ac474d418629a0bba19d925698d72cf8
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61650491"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>accessReviewNotificationRecipientItem resource type

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


Представляет событие уведомления об уведомлении о просмотре доступа Azure [AD](accessreviewsv2-overview.md) в экземпляре проверки. Этот элемент содержит тип шаблона электронной почты и свойства получателей, чтобы включить отправку определенных типов уведомлений для данного экземпляра [обзора доступа.](accessreviewinstance.md)

## <a name="properties"></a>Свойства

| Свойство                     | Тип     | Описание                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |Строка  | Указывает тип отправки электронной почты для проверки доступа. Поддерживаемый тип шаблона — это отправка получателям уведомлений о `CompletedAdditionalRecipients` завершении проверки.|
| notificationRecipientScope |[accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)  | Определяет получателя сообщения уведомления.|

## <a name="relationships"></a>Отношения
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
