---
title: Тип ресурса АадусернотификатионреЦипиент
description: Представляет получателя Azure Active Directory (Azure AD) для уведомления, отправленного в веб-канале активности Microsoft Teams.
author: RamjotSingh
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 118951336a031548a557f94df8b2b2068e415408
ms.sourcegitcommit: 6201b3a5646f640f25a68ab033eca9eb60ccd05e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/21/2020
ms.locfileid: "49377570"
---
# <a name="aadusernotificationrecipient-resource-type"></a>Тип ресурса АадусернотификатионреЦипиент

Пространство имен: microsoft.graph

Представляет получателя Azure Active Directory (Azure AD) для уведомления, отправленного в веб-канале активности Microsoft Teams.

Наследуется от [теамворкнотификатионреЦипиент](teamworknotificationrecipient.md).

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|userId|String|Идентификатор пользователя Azure AD. Для получения этого идентификатора используйте метод [List Users](../api/user-list.md) .|

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

