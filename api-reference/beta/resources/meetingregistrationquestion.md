---
title: тип ресурса meetingRegistrationQuestion
description: Представляет настраиваемый вопрос регистрации, помимо имени, фамилии и адреса электронной почты, связанный с собраниемРегистрация.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 42645be07a3540294906cb03fb7b28c080bbd0ed
ms.sourcegitcommit: c3f849e5a052b1926373a4b316ec303250e6d09e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/15/2021
ms.locfileid: "60370393"
---
# <a name="meetingregistrationquestion-resource-type"></a>тип ресурса meetingRegistrationQuestion

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет настраиваемый вопрос регистрации, помимо имени, фамилии и адреса электронной почты, связанный с [собраниемRegistration.](meetingRegistration.md)

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
| :----- | :---------- | :---------- |
|[Список](../api/meetingregistration-list-customquestions.md) | [коллекция meetingRegistrationQuestion](meetingregistrationquestion.md) | Список всех пользовательских вопросов регистрации. |
|[Создание](../api/meetingregistration-post-customquestions.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | Создайте настраиваемый вопрос регистрации. |
|[получение](../api/meetingregistrationquestion-get.md); | [meetingRegistrationQuestion](meetingregistrationquestion.md) | Получите настраиваемый вопрос регистрации. |
|[Обновление](../api/meetingregistrationquestion-update.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | Обновление настраиваемой регистрации. |
|[Удаление](../api/meetingregistrationquestion-delete.md) | [meetingRegistrationQuestion](meetingregistrationquestion.md) | Удаление настраиваемой регистрации вопроса. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| answerInputType | [answerInputType](#answerinputtype-values) | Ответ на тип ввода пользовательского вопроса регистрации. |
| answerOptions | Коллекция объектов string | Варианты ответа при **ответеInputType** `radioButton` . |
| displayName | String | Отображение имени настраиваемого вопроса регистрации. |
| id | String | ID пользовательского вопроса регистрации. Только для чтения. |
| isRequired | Boolean | Указывает, требуется ли этот вопрос. Значение по умолчанию — `false`. |

### <a name="answerinputtype-values"></a>answerInputType values

| Значение              | Описание |
|--------------------|-------------|
| text | Вопрос принимает текстовый ответ одной строки. |
| radioButton | Вопрос принимает ответ, выбранный из кнопок радио. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistrationQuestion"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "isRequired": "Boolean",
  "answerInputType": { "@odata.type": "microsoft.graph.answerInputType" },
  "answerOptions": [ "String" ],
}
```
