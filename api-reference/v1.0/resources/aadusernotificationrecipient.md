---
title: тип ресурса aadUserNotificationRecipient
description: Представляет получателя пользователя Azure Active Directory (Azure AD) с уведомлением, отправленным в канале действий Microsoft Teams.
author: eddie-lee-msft
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: dadb08dad99f6c4fd6857e8e60f457ea51811de1
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474147"
---
# <a name="aadusernotificationrecipient-resource-type"></a>тип ресурса aadUserNotificationRecipient

Пространство имен: microsoft.graph

Представляет получателя пользователя Azure Active Directory (Azure AD) с уведомлением, отправленным в канале действий Microsoft Teams.

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

