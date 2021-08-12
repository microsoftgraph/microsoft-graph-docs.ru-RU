---
title: тип ресурса aadUserNotificationRecipient
description: Представляет получателя Azure Active Directory пользователя Azure AD, отправимого в канале Microsoft Teams действий.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: bb5d95c36fb362af6d4f66c1e18a4dcb768c1b204a4e2f70f24f5afe80545483
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54230853"
---
# <a name="aadusernotificationrecipient-resource-type"></a>тип ресурса aadUserNotificationRecipient

Пространство имен: microsoft.graph

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

