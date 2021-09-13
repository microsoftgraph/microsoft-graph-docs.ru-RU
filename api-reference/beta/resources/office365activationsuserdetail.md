---
title: тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.localizationpriority: medium
ms.prod: reports
author: sarahwxy
doc_type: resourcePageType
ms.openlocfilehash: c70d67519ed43c36fa4bcc4df1a8d18566d732fd
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59057126"
---
# <a name="office365activationsuserdetail-resource-type"></a>тип ресурса office365ActivationsUserDetail

Пространство имен: microsoft.graph

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | Дата                                     | Последняя дата контента.          |
| userPrincipalName    | String                                   | Имя участника-пользователя. Это имя для входа через Интернет по стандарту RFC 822. В соответствии с соглашением оно должно указывать на имя пользователя для электронной почты. Общий формат: псевдоним@домен. При этом домен должен входить в коллекцию проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. |
| displayName          | String                                   | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. |
| userActivationCounts | [коллекция userActivationCounts](../resources/useractivationcounts.md) | Последняя активация продукта пользователя рассчитывается на всех платформах для всех типов продуктов. |

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


