---
title: Тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
ms.openlocfilehash: 9cf0f7f841584654176c0069fb0403a86615bfd5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27076984"
---
# <a name="office365activationsuserdetail-resource-type"></a>Тип ресурса office365ActivationsUserDetail

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Description                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | Date                                     | Последняя дата контента.          |
| userPrincipalName    | String                                   | Основной имя пользователя (UPN) пользователя. Имя участника-пользователя — это имя для входа характерном для Интернета для пользователя на основании Интернета standard RFC 822. В соответствии с соглашением это сопоставление имен пользователей электронной почты. Общие имеет формат alias@domain, где должны быть представлены в семейство подтвержденным доменов из домена. Это свойство обязательно указывать при создании пользователя. |
| displayName          | String                                   | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. |
| userActivationCounts | [userActivationCounts](../resources/useractivationcounts.md) коллекции | Новейшие активации пользователя счетчиков для всех платформ для всех типов назначенный продукта. |

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
