---
title: тип ресурса meetingRegistration
description: Содержит сведения о регистрации собраний в Интернете.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: ab41bebd48947851721e2adc78a07f01fc522117
ms.sourcegitcommit: 15956da1b4a7d523363ffa8afb5e2059fbf680ce
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/01/2022
ms.locfileid: "62291964"
---
# <a name="meetingregistration-resource-type"></a>тип ресурса meetingRegistration

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Содержит сведения о регистрации собрания в Интернете, например [вебинар Microsoft Teams вебинар](https://support.microsoft.com/office/get-started-with-teams-webinars-42f3f874-22dc-4289-b53f-bbc1a69013e3). 

Наследуется [от meetingRegistrationBase](meetingregistrationbase.md).

## <a name="methods"></a>Методы

| Метод | Возвращаемый тип | Описание |
| :----- | :---------- | :---------- |
|[Создание](../api/meetingregistration-post.md) | [meetingRegistration](meetingregistration.md) | Создание и включить регистрацию для собрания в Интернете. |
|[Получение](../api/meetingregistration-get.md); | [meetingRegistration](meetingregistration.md) | Извлечение сведений о регистрации собрания. |
|[Обновление](../api/meetingregistration-update.md) | [meetingRegistration](meetingregistration.md) | Обновление сведений о регистрации собрания. |
|[удаление](../api/meetingregistration-delete.md); | [meetingRegistration](meetingregistration.md) | Отключить и удалить регистрацию для собрания в Интернете. |

## <a name="properties"></a>Свойства

| Свойство | Тип | Описание |
| :------- | :--- | :---------- |
| allowedRegistrant | [meetingAudience](#meetingaudience-values) | Указывает, кто может зарегистрироваться для собрания. |
| description | String | Описание собрания. |
| endDateTime | Даты и время | Время окончания собрания в UTC. |
| registrationPageViewCount | Int32 | Количество посещений страницы регистрации. Только для чтения. |
| registrationPageWebUrl | String | URL-адрес страницы регистрации. Только для чтения. |
| динамики | [meetingSpeaker](meetingSpeaker.md) collection | Сведения спикера собрания. |
| startDateTime | Даты и время | Время начала собрания в UTC. |
| subject | String | Тема собрания. |

### <a name="meetingaudience-values"></a>значения meetingAudience

| Значение              | Описание |
| ------------------ | ----------- |
| все           | Зарегистрироваться на собрание может каждый. |
| organization       | Все в организации организатора могут зарегистрироваться на собрание. |
| unknownFutureValue | Эволюционирующее значение sentinel. Не следует использовать. |

## <a name="relationships"></a>Связи

| Связь | Тип | Описание |
| ------------ | ---- | ----------- |
| customQuestions | [коллекция meetingRegistrationQuestion](meetingRegistrationQuestion.md)| Настраиваемые вопросы регистрации. |
| регистраторы | [коллекция meetingRegistrant](meetingRegistrant.md) | Регистраторы собрания в Интернете. |

## <a name="json-representation"></a>Представление JSON

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.meetingRegistration"
}-->

```json
{
  "allowedRegistrant": { "@odata.type": "microsoft.graph.meetingAudience" },
  "description": "String",
  "endDateTime": "String (timestamp)",
  "registrationPageViewCount": "Int32",
  "registrationPageWebUrl": "String",
  "speakers": [{ "@odata.type": "microsoft.graph.meetingSpeaker" }],
  "startDateTime": "String (timestamp)",
  "subject": "String",

  "customQuestions": [{ "@odata.type": "microsoft.graph.meetingRegistrationQuestion" }],
  "registrants": [{ "@odata.type": "microsoft.graph.meetingRegistrant" }]
}
```
