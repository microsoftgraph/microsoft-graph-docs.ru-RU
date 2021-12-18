---
title: тип ресурса meetingRegistrant
description: Представляет регистратор собрания, который зарегистрировался на собрании в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9d3a55ddd14cb33b02a69fb09c0721f3c9986fdb
ms.sourcegitcommit: ba46f9f77d1e0eb9c7f5b2f4366534bfcf99d9c0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2021
ms.locfileid: "61561350"
---
# <a name="meetingregistrant-resource-type"></a>тип ресурса meetingRegistrant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет регистратор собрания, который зарегистрировался на собрании [в Интернете.](onlinemeeting.md) 

Наследует от [meetingRegistrantBase](meetingregistrantbase.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
| :----- | :---------- | :---------- |
|[Список](../api/meetingregistration-list-registrants.md) | [meetingRegistrant](meetingregistrant.md) | Список всех регистраторов, которые зарегистрировались на собрании. |
|[Создание](../api/meetingregistration-post-registrants.md) | [meetingRegistrant](meetingregistrant.md) | Регистрация регистратора на собрании в Интернете. |
|[удаление](../api/meetingregistrant-delete.md); | [meetingRegistrant](meetingregistrant.md) | Отодинить регистратора от собрания в Интернете. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| customQuestionAnswers | [коллекция customQuestionAnswer](customQuestionAnswer.md) | Ответ регистратора на настраиваемые вопросы. |
| email | String | Адрес электронной почты регистратора. |
| firstName | Строка | Имя регистратора. |
| id | Строка | Уникальный идентификатор регистратора. Только для чтения. |
| joinWebUrl | Строка | Уникальный веб-URL-адрес для регистратора, который должен присоединиться к собранию. Только для чтения. |
| lastName | Строка | Фамилия регистратора. |
| registrationDateTime | Строка | Время в UTC, когда регистратор регистрирует собрание. Только для чтения. |
| status | [meetingRegistrantStatus](#meetingregistrantstatus-values) | Состояние регистрации регистратора. Только для чтения. |

### <a name="meetingregistrantstatus-values"></a>значения meetingRegistrantStatus

| Значение              | Описание |
|--------------------|-------------|
| зарегистрирована | Регистратор зарегистрировался на собрании. |
| отменено | Регистратор отменил их регистрацию. |
| обработка | Промежуточный статус, указывающий на состояние, обрабатывается. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistrant"
}-->

```json
{
  "id": "String",
  "firstName": "String (timestamp)",
  "email": "String",
  "lastName": "String",
  "joinWebUrl": "String",
  "registrationDateTime": "String (timestamp)",
  "status": { "@odata.type": "microsoft.graph.meetingRegistrantStatus" },
  "customQuestionAnswers": [{ "@odata.type": "microsoft.graph.customQuestionAnswer" }]
}
```
