---
title: Тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 45219f7666d4432bcdb2b409491338b94650a726
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522479"
---
# <a name="office365activationsuserdetail-resource-type"></a>Тип ресурса office365ActivationsUserDetail

Пространство имен: Microsoft. Graph

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| репортрефрешдате    | Дата                                     | Самая поздняя дата контента.          |
| userPrincipalName    | String                                   | Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. |
| displayName          | Строка                                   | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. |
| усерактиватионкаунтс | Коллекция [усерактиватионкаунтс](../resources/useractivationcounts.md) | Последние числа активаций на всех платформах для всех типов назначенных продуктов пользователя. |

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserDetail"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "userPrincipalName": "String", 
  "displayName": "String", 
  "userActivationCounts": [{"@odata.type":"microsoft.graph.userActivationCounts"}]
}
```
