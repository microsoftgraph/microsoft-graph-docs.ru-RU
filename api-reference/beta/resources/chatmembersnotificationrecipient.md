---
title: тип ресурса chatMembersNotificationRecipient
description: Представляет получателя уведомления, отправленного в канале Microsoft Teams действий. Получатель состоит из участников чата.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 3743d9d37e934cd61f699febfcc148afb8e84e98
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211398"
---
# <a name="chatmembersnotificationrecipient-resource-type"></a>тип ресурса chatMembersNotificationRecipient

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет получателя уведомления, отправленного в канале Microsoft Teams действий. Получатель состоит из участников чата.

Наследует [от teamworkNotificationRecipient](teamworknotificationrecipient.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|chatId|String|Идентификатор чата.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.chatMembersNotificationRecipient"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.chatMembersNotificationRecipient",
  "chatId": "String"
}
```

