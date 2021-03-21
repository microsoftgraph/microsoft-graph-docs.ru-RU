---
title: тип ресурсов relatedContact
description: Запись контактов, связанная с educationUser, который предоставляет информацию для опекунов, помощников, врачей и так далее.
author: mmast-msft
ms.author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 37c494d58896af34c1da12e6e500a0561d877911
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960336"
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
| displayName   | Строка              | Имя контакта. Обязательный.                                                                                                             |
| accessConsent | Boolean             | Указывает, было ли получено согласие пользователя на доступ к данным учащихся.                                                                      |
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
