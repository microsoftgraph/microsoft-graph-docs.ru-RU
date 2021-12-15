---
title: тип ресурса bookingCustomQuestion
description: Представляет настраиваемый вопрос для bookingBusiness.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 9a9f88d7ee5fe20d1dc5b4033353b2ac7b744878
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525130"
---
# <a name="bookingcustomquestion-resource-type"></a>тип ресурса bookingCustomQuestion

Пространство имен: microsoft.graph

Представляет настраиваемый вопрос для [bookingBusiness](bookingbusiness.md).

## <a name="methods"></a>Методы

| Метод                                                                         | Тип возвращаемых данных                                                               | Описание                                                                                                       |
| :----------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------- |
| [Список bookingCustomQuestions](../api/bookingbusiness-list-customquestions.md)  | [коллекция bookingCustomQuestion](../resources/bookingcustomquestion.md) | Получите список объектов [bookingCustomQuestion](../resources/bookingcustomquestion.md) и их свойств.    |
| [Создание bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md) | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Создайте новый [объект bookingCustomQuestion.](../resources/bookingcustomquestion.md)                               |
| [Получить bookingCustomQuestion](../api/bookingcustomquestion-get.md)               | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Ознакомьтесь с свойствами и отношениями объекта [bookingCustomQuestion.](../resources/bookingcustomquestion.md) |
| [Обновление bookingCustomQuestion](../api/bookingcustomquestion-update.md)         | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Обновление свойств объекта [bookingCustomQuestion.](../resources/bookingcustomquestion.md)                 |
| [Удаление bookingCustomQuestion](../api/bookingcustomquestion-delete.md)         | Нет                                                                      | Удаление [объекта bookingCustomQuestion.](../resources/bookingcustomquestion.md)                                  |

## <a name="properties"></a>Свойства

| Свойство        | Тип              | Описание                                                                                               |
| :-------------- | :---------------- | :-------------------------------------------------------------------------------------------------------- |
| answerInputType | answerInputType   | Ожидаемый тип ответа. Допустимые значения: `text`, `radioButton`, `unknownFutureValue`.     |
| answerOptions   | Коллекция строк | Список возможных значений ответов.                                                                    |
| displayName     | Строка            | Вопрос. |
| id              | Строка            | ID настраиваемого вопроса. Наследуется от [сущности](../resources/entity.md).                           |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
  "openType": false
}
-->

```json
{
  "@odata.type": "#microsoft.graph.bookingCustomQuestion",
  "id": "String (identifier)",
  "displayName": "String",
  "answerInputType": {"@odata.type": "microsoft.graph.answerInputType"},
  "answerOptions": ["String"]
}
```
