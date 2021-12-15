---
title: тип ресурса bookingCustomQuestion
description: Представляет настраиваемый вопрос для bookingBusiness.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: 65baf5850be3dc5c9b86c24078061b54dff7d1aa
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526983"
---
# <a name="bookingcustomquestion-resource-type"></a>тип ресурса bookingCustomQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемый вопрос для [bookingBusiness](bookingbusiness.md).

Наследует [от bookingNamedEntity](../resources/bookingnamedentity.md).

## <a name="methods"></a>Методы

| Метод                                                                         | Тип возвращаемых данных                                                               | Описание                                                                                                       |
| :----------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------- |
| [Список bookingCustomQuestions](../api/bookingbusiness-list-customquestions.md)            | [коллекция bookingCustomQuestion](../resources/bookingcustomquestion.md) | Получите список объектов [bookingCustomQuestion](../resources/bookingcustomquestion.md) и их свойств.    |
| [Создание bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md) | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Создайте новый [объект bookingCustomQuestion.](../resources/bookingcustomquestion.md)                               |
| [Получить bookingCustomQuestion](../api/bookingcustomquestion-get.md)               | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Ознакомьтесь с свойствами и отношениями объекта [bookingCustomQuestion.](../resources/bookingcustomquestion.md) |
| [Обновление bookingCustomQuestion](../api/bookingcustomquestion-update.md)         | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Обновление свойств объекта [bookingCustomQuestion.](../resources/bookingcustomquestion.md)                 |
| [Удаление bookingCustomQuestion](../api/bookingcustomquestion-delete.md)         | Нет                                                                      | Удаление [объекта bookingCustomQuestion.](../resources/bookingcustomquestion.md)                                  |

## <a name="properties"></a>Свойства

| Свойство        | Тип              | Описание                                                                                               |
| :-------------- | :---------------- | :-------------------------------------------------------------------------------------------------------- |
| answerInputType | answerInputType   | Ожидаемый тип ответа. Допустимые значения: `text`, `radioButton`, `unknownFutureValue`.     |
| answerOptions   | Коллекция строк | Список возможных значений ответов.                                                                    |
| displayName     | Строка            | Вопрос. Наследуется [от bookingNamedEntity](../resources/bookingnamedentity.md). |
| id              | Строка            | ID настраиваемого вопроса. Наследуется от [сущности](../resources/entity.md).                           |

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bookingCustomQuestion",
  "baseType": "microsoft.graph.bookingNamedEntity",
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
