---
title: Тип ресурса bookingCustomQuestion
description: Представляет пользовательский вопрос для bookingBusiness.
author: razortbone
ms.localizationpriority: medium
ms.prod: bookings
doc_type: resourcePageType
ms.openlocfilehash: cf672b93e30b6351d3f543b5cc9341d53fea1d5d
ms.sourcegitcommit: 8253b79a9fdfea723899860492219eaeb9f74e3d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/18/2022
ms.locfileid: "66160638"
---
# <a name="bookingcustomquestion-resource-type"></a>Тип ресурса bookingCustomQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет пользовательский вопрос для [bookingBusiness](bookingbusiness.md).

Наследуется от [bookingNamedEntity](../resources/bookingnamedentity.md).

## <a name="methods"></a>Методы

| Метод                                                                         | Тип возвращаемых данных                                                               | Описание                                                                                                       |
| :----------------------------------------------------------------------------- | :------------------------------------------------------------------------ | :---------------------------------------------------------------------------------------------------------------- |
| [Перечисление bookingCustomQuestions](../api/bookingbusiness-list-customquestions.md)            | [Коллекция bookingCustomQuestion](../resources/bookingcustomquestion.md) | Получение списка объектов [bookingCustomQuestion](../resources/bookingcustomquestion.md) и их свойств.    |
| [Создание bookingCustomQuestion](../api/bookingbusiness-post-customquestions.md) | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Создайте объект [bookingCustomQuestion](../resources/bookingcustomquestion.md) .                               |
| [Получение bookingCustomQuestion](../api/bookingcustomquestion-get.md)               | [bookingCustomQuestion](../resources/bookingcustomquestion.md)            | Чтение свойств и связей объекта [bookingCustomQuestion](../resources/bookingcustomquestion.md) . |
| [Обновление bookingCustomQuestion](../api/bookingcustomquestion-update.md)         | Нет     | Обновление свойств объекта [bookingCustomQuestion](../resources/bookingcustomquestion.md) .                 |
| [Удаление bookingCustomQuestion](../api/bookingcustomquestion-delete.md)         | Нет                                                                      | Удаление объекта [bookingCustomQuestion](../resources/bookingcustomquestion.md) .                                  |

## <a name="properties"></a>Свойства

| Свойство        | Тип              | Описание                                                                                               |
| :-------------- | :---------------- | :-------------------------------------------------------------------------------------------------------- |
| answerInputType | answerInputType   | Ожидаемый тип ответа. Допустимые значения: `text`, `radioButton`, `unknownFutureValue`.     |
| answerOptions   | Коллекция String | Список возможных значений ответов.                                                                    |
| displayName     | Строка            | Вопрос. Наследуется [от bookingNamedEntity](../resources/bookingnamedentity.md). |
| id              | Строка            | Идентификатор пользовательского вопроса. Наследуется от [сущности](../resources/entity.md).                           |

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
