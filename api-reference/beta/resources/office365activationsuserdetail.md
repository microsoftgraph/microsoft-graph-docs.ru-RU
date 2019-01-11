---
title: Тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.openlocfilehash: f87a5b32b08466428f0f6f0246a4b8d4c20e97be
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877338"
---
# <a name="office365activationsuserdetail-resource-type"></a>Тип ресурса office365ActivationsUserDetail

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| reportRefreshDate    | Date                                     | Последняя дата контента.          |
| userPrincipalName    | Строка                                   | Основной имя пользователя (UPN) пользователя. Имя участника-пользователя — это имя для входа характерном для Интернета для пользователя на основании Интернета standard RFC 822. В соответствии с соглашением это сопоставление имен пользователей электронной почты. Общие имеет формат alias@domain, где должны быть представлены в семейство подтвержденным доменов из домена. Это свойство обязательно указывать при создании пользователя. |
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
