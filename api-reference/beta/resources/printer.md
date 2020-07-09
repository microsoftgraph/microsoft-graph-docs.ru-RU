---
title: Тип ресурса Printer
description: Представляет физическое устройство печати, зарегистрированное в универсальной службе печати. Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 6573f17753a3c9b487324def9973bddd0759ed4b
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091440"
---
# <a name="printer-resource-type"></a>Тип ресурса Printer

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет физическое устройство печати, зарегистрированное в универсальной службе печати. Ресурсы принтера можно использовать для управления заданиями печати, параметрами принтеров, метаданными принтера и состоянием регистрации.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип | Описание |
|:-------------|:------------|:------------|
| [Создание](../api/printer-create.md); | [принтеркреатеоператион](printerCreateOperation.md) | Создание (регистрация) нового принтера с универсальной печатью. |
| [Get](../api/printer-get.md) | [Printer](printer.md) | Чтение свойств и связей объекта Printer. |
| [Update](../api/printer-update.md) | [Printer](printer.md) | Обновление объекта Printer. |
| [Delete](../api/printer-delete.md) | Нет | Отмените регистрацию физического принтерфром в универсальной службе печати. |
| [getCapabilities](../api/printer-getcapabilities.md) | [принтеркапабилитиес](printercapabilities.md) | Получение списка возможностей принтера. |
| [ресетдефаултс](../api/printer-resetdefaults.md) | Отсутствует | Сброс параметров принтера по умолчанию. |
| [Список заданий](../api/printer-list-jobs.md) | Коллекция [printJob](printjob.md) | Получение списка заданий печати, помещенных в очередь для обработки принтером. |
| [Создание задания](../api/printer-post-jobs.md) | [printJob](printjob.md) | Создание нового задания печати для принтера. Чтобы начать печать задания, используйте [стартпринтжоб](../api/printjob-startprintjob.md). |
| [Список соединителей](../api/printer-list-connectors.md) | Коллекция [принтконнектор](printconnector.md) | Получение списка соединителей, с которыми связан этот принтер. |
| [Список allowedUsers](../api/printer-list-allowedusers.md) | Коллекция [принтусеридентити](printuseridentity.md) | Получение списка пользователей, которым предоставлен доступ к отправку заданий печати на связанный принтер. |
| [Добавление allowedUser](../api/printer-post-allowedusers.md) | Отсутствует | Предоставьте заданному пользователю доступ на отправку заданий печати на связанный принтер. |
| [Удаление allowedUser](../api/printer-delete-alloweduser.md) | Отсутствует | Отзыв доступа к принтеру для указанного пользователя. |
| [Список allowedGroups](../api/printer-list-allowedgroups.md) | Коллекция [принтидентити](printidentity.md) | Получение списка групп, которым предоставлен доступ на отправку заданий печати на связанный принтер. |
| [Добавление allowedGroup](../api/printer-post-allowedgroups.md) | Отсутствует | Предоставление указанному групповому доступу на отправку заданий печати на связанный принтер. |
| [Удаление allowedGroup](../api/printer-delete-allowedgroup.md) | Отсутствует | Отзыв доступа к принтеру из указанной группы. |
| [Список Тасктригжерс](../api/printer-list-tasktriggers.md) | Отсутствует | Список [принттасктригжерс](printtasktrigger.md) , связанных с этим принтером. |
| [Создание Тасктригжер](../api/printer-post-tasktriggers.md) | [принттасктригжер](printtasktrigger.md) | Создание [принттасктригжер](printtasktrigger.md) , выполняемого при возникновении событий печати. |
| [Удаление Тасктригжер](../api/printer-delete-tasktrigger.md) | Отсутствует | Удаление [принттасктригжер](printtasktrigger.md) , связанного с принтером. |

## <a name="properties"></a>Свойства
| Свойство     | Тип        | Описание |
|:-------------|:------------|:------------|
|id|String|Идентификатор документа. Только для чтения.|
|displayName|Строка|Имя принтера.|
|manufacturer|String|Производитель, сообщаемый принтером. Только для чтения.|
|model|String|Имя модели, сообщаемое принтером. Только для чтения.|
|регистереддатетиме|DateTimeOffset|Значение DateTimeOffset при регистрации принтера. Только для чтения.|
|status|[принтерстатус](printerstatus.md)|Состояние обработки принтера, включая ошибки. Только для чтения.|
|IsShared|Boolean|Значение true, если принтер является общим; в противном случае — false. Только для чтения.|
|исакцептингжобс|Boolean|Принимает ли принтер новые задания печати.|
|location|[принтерлокатион](printerlocation.md)|Физическое и/или организационное расположение принтера.|
|по умолчанию|[принтердефаултс](printerdefaults.md)|Параметры печати по умолчанию для принтера.|

## <a name="relationships"></a>Связи
| Связь | Тип        | Описание |
|:-------------|:------------|:------------|
|работе|Коллекция [printJob](printjob.md)| Список заданий, помещенных в очередь на печать принтером.|
|shares|Коллекция [принтершаре](printershare.md)| Список Принтершарес, связанных с принтером. Только для чтения. Допускается значение null.|
|аудиовыход|[принтконнектор](printconnector.md)|Соединители, связанные с принтером.|
|алловедусерс|Коллекция [принтусеридентити](printuseridentity.md)|Пользователи, у которых есть доступ к печати с помощью принтера.|
|алловедграупс|[принтидентити](printidentity.md)|Группы, у которых пользователи имеют доступ к печати с помощью принтера.|
|тасктригжерс|Коллекция [принттасктригжер](printtasktrigger.md)|Список триггеров задач, связанных с принтером.|

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printer",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String",
  "manufacturer": "String",
  "model": "String",
  "isShared": true,
  "registeredDateTime": "String (timestamp)",
  "acceptingJobs": true,
  "registeredBy": {"@odata.type": "microsoft.graph.printUserIdentity"},
  "location": {"@odata.type": "microsoft.graph.printerLocation"},
  "status": {"@odata.type": "microsoft.graph.printerStatus"},
  "defaults": {"@odata.type": "microsoft.graph.printerDefaults"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printer resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
