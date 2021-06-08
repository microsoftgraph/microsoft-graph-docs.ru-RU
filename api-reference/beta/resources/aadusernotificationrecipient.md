---
title: тип ресурса aadUserNotificationRecipient
description: Представляет получателя Azure Active Directory пользователя Azure AD, отправимого в канале Microsoft Teams действий.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ec8e05a09af27ca6092da24e13a604fdd7e013f4
ms.sourcegitcommit: a2d81138de2a0404e611fbb535679199477ef3d5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/08/2021
ms.locfileid: "52813201"
---
# <a name="aadusernotificationrecipient-resource-type"></a>тип ресурса aadUserNotificationRecipient

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет получателя Azure Active Directory пользователя Azure AD, отправимого в канале Microsoft Teams действий.

Наследует [от teamworkNotificationRecipient](teamworknotificationrecipient.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Идентификатор пользователя Azure AD. Чтобы получить [этот](../api/user-list.md) ID, используйте метод пользователей списка.|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.aadUserNotificationRecipient"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.aadUserNotificationRecipient",
  "userId": "String"
}
```

