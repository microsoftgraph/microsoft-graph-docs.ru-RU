---
title: тип ресурса meetingRegistrant
description: Представляет регистратор собрания, который зарегистрировался на собрании в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dbc90ecc79258ad150077d474fcdd8d4b29f6db6
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2021
ms.locfileid: "60369526"
---
# <a name="meetingregistrant-resource-type"></a>тип ресурса meetingRegistrant

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет регистратор собрания, который зарегистрировался на собрании [в Интернете.](onlinemeeting.md)

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
| :----- | :---------- | :---------- |
|[Список](../api/meetingregistration-list-registrants.md) | [meetingRegistrant](meetingregistrant.md) | Список всех регистраторов, которые зарегистрировались на собрании. |
|[Создание](../api/meetingregistration-post-registrants.md) | [meetingRegistrant](meetingregistrant.md) | Регистрация регистратора на собрании в Интернете. |
|[Удаление](../api/meetingregistrant-delete.md) | [meetingRegistrant](meetingregistrant.md) | Отодинить регистратора от собрания в Интернете. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| customQuestionAnswers | [коллекция customQuestionAnswer](customQuestionAnswer.md) | Ответ регистратора на настраиваемые вопросы. |
| email | String | Адрес электронной почты регистратора. |
| firstName | String | Имя регистратора. |
| id | String | ID регистратора. Только для чтения. |
| joinWebUrl | String | Уникальный веб-URL-адрес для регистратора, который должен присоединиться к собранию. Только для чтения. |
| lastName | String | Фамилия регистратора. |
| registrationDateTime | String | Время в UTC, когда регистратор регистрирует собрание. Только для чтения. |
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
