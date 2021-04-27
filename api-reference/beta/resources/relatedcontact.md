---
title: тип ресурсов relatedContact
description: Запись контактов, связанная с educationUser, который предоставляет информацию для опекунов, помощников, врачей и так далее.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4859492f016b88a39c375d3556270f5496b8b318
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035955"
---
# <a name="relatedcontact-resource-type"></a>тип ресурсов relatedContact

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Запись контактов, связанная с [educationUser,](../resources/educationuser.md) который предоставляет информацию для опекунов, помощников, врачей и так далее.

## <a name="methods"></a>Методы

| Метод                                    | Возвращаемый тип                   | Описание                                                             |
| :---------------------------------------- | :---------------------------- | :---------------------------------------------------------------------- |
| [Обновление](../api/relatedcontact-update.md) | **коллекция relatedContact** | Обновление **связанныхContacts** для [educationUser](educationuser.md) |

## <a name="properties"></a>Свойства

| Свойство      | Тип                | Описание                                                                                                                                |
| :------------ | :------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| displayName   | String              | Имя контакта. Обязательный.                                                                                                             |
| accessConsent | Логический             | Указывает, было ли получено согласие пользователя на доступ к данным учащихся.                                                                      |
| emailAddress  | String              | Адрес электронной почты контакта.                                                                                                              |
| mobilePhone   | String              | Номер мобильного телефона контакта.                                                                                                        |
| Отношение  | contactRelationship | Отношение к пользователю. Возможные значения: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`. |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.relatedContact"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.relatedContact",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String",
  "accessConsent": "Boolean"
}
```
