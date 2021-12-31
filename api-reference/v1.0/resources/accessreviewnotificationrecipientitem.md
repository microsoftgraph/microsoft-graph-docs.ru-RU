---
title: accessReviewNotificationRecipientItem resource type
description: Определяет пользователей или группы, которые будут получать уведомления о просмотре доступа к уведомлениям.
author: isabelleatmsft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 7f63f9cfe3e1233407d0aaf966d9e2c0d933da26
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61649692"
---
# <a name="accessreviewnotificationrecipientitem-resource-type"></a>accessReviewNotificationRecipientItem resource type

Пространство имен: microsoft.graph

Представляет событие уведомления об уведомлении о просмотре доступа Azure [AD](accessreviewsv2-overview.md) в экземпляре проверки. Этот элемент содержит тип шаблона электронной почты и свойства получателей, чтобы включить отправку определенных типов уведомлений для данного экземпляра [обзора доступа.](accessreviewinstance.md)

## <a name="properties"></a>Свойства

| Свойство                     | Тип     | Описание                          |
| :--------------------------- | :------  | :----------                          |
| notificationTemplateType  |Строка  | Указывает тип отправки электронной почты для проверки доступа. Поддерживаемый тип шаблона , который отправляет уведомления о `CompletedAdditionalRecipients` завершении проверки получателям.|
| notificationRecipientScope |[accessReviewNotificationRecipientScope](../resources/accessreviewnotificationrecipientscope.md)  | Определяет получателя сообщения уведомления.|

## <a name="relationships"></a>Отношения
Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

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
