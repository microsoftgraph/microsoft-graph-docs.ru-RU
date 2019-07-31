---
title: Тип ресурса office365ActivationsUserDetail
description: Ниже указано представление ресурса в формате JSON.
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 2ced56fdc8f2ed877368163e36588e3d4983d95e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009533"
---
# <a name="office365activationsuserdetail-resource-type"></a>Тип ресурса office365ActivationsUserDetail

## <a name="properties"></a>Свойства

| Свойство             | Тип                                     | Описание                              |
| :------------------- | :--------------------------------------- | ---------------------------------------- |
| Репортрефрешдате    | Дата                                     | Самая поздняя дата контента.          |
| userPrincipalName    | String                                   | Имя участника-пользователя (UPN). UPN — это имя входа в стиле Интернета для пользователя на основе стандартного стандарта RFC 822. По соглашению он должен сопоставляться с именем электронной почты пользователя. Общий формат — псевдоним @ Domain, где домен должен присутствовать в коллекции проверенных доменов клиента. Это свойство обязательно указывать при создании пользователя. |
| displayName          | Строка                                   | Имя пользователя, отображаемое в адресной книге. Обычно это сочетание имени, отчества и фамилии пользователя. Это свойство необходимо указывать при создании пользователя. Его невозможно удалить при обновлении. |
| Усерактиватионкаунтс | Коллекция [усерактиватионкаунтс](../resources/useractivationcounts.md) | Последние числа активаций на всех платформах для всех типов назначенных продуктов пользователя. |

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
