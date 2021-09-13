---
title: тип ресурса aadUserNotificationRecipient
description: Представляет получателя Azure Active Directory пользователя Azure AD, отправимого в канале Microsoft Teams действий.
author: eddie-lee-msft
ms.localizationpriority: medium
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 4588b0d17dc099ee65cedeba52bd5cbd1edf7bae
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59021787"
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

