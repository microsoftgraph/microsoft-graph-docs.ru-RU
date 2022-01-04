---
title: Тип ресурса directoryObject
description: Представляет объект Azure Active Directory. Тип directoryObject является базовым типом для многих других типов объектов каталогов.
ms.localizationpriority: high
author: keylimesoda
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 545ab52782c8bec83f711faf3928d10d4c3105c1
ms.sourcegitcommit: 00ac72f7b1cdde4f71ff332c2e7953908ef9de52
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/04/2022
ms.locfileid: "61711593"
---
# <a name="directoryobject-resource-type"></a>Тип ресурса directoryObject

Пространство имен: microsoft.graph

Представляет объект Azure Active Directory. Тип **directoryObject** является базовым типом для многих других типов объектов каталогов.

## <a name="methods"></a>Методы

| Метод       | Возвращаемый тип  |Описание|
|:---------------|:--------|:----------|
|[Получение объекта directoryObject](../api/directoryobject-get.md) | [directoryObject](directoryobject.md) |Чтение свойств объекта каталога.|
|[Удаление объекта directoryObject](../api/directoryobject-delete.md) | Нет |Удаление объекта каталога. |
|[Получение доступных свойств расширения](../api/directoryobject-getavailableextensionproperties.md)|Коллекция [extensionProperty](../resources/extensionproperty.md)|Получение полного или отфильтрованного списка свойств расширения каталога, которые зарегистрированы в каталоге.|
|[checkMemberGroups](../api/directoryobject-checkmembergroups.md)|Коллекция String|Проверка участия в указанном списке групп и возвращение из этого списка тех групп, в которых состоит указанный пользователь, группа, субъект-служба, контакт организации, устройство или объект каталога. Это транзитивная проверка.|
|[getMemberGroups](../api/directoryobject-getmembergroups.md)|Коллекция String|Возвращение всех групп, в которых состоит пользователь, группа, субъект-служба, контакт организации, устройство или объект каталога. Это транзитивная проверка.|
|[checkMemberObjects](../api/directoryobject-checkmemberobjects.md)|Коллекция String|Проверка участия в списке ролей группы, административных единиц или каталога для указанного пользователя, группы, устройства, контакта организации или объекта каталога. Это транзитивный метод.|
|[getMemberObjects](../api/directoryobject-getmemberobjects.md)|Коллекция String| Возвращение всех ролей групп, административных единиц и каталога, в которых состоит пользователь, группа, устройство, контакт организации или объект каталога. Это транзитивная проверка. |
|[getByIds](../api/directoryobject-getbyids.md) | Коллекция [directoryObject](directoryobject.md) | Получение набора объектов каталога на основе указанных идентификаторов. |
|[validateProperties](../api/directoryobject-validateproperties.md)|JSON| Проверка соответствия отображаемого имени или почтового псевдонима группы Microsoft 365 политикам именования. |
|delta|Коллекция [directoryObject](directoryObject.md)| Получение добавочных изменений для объектов каталогов, например для [пользователей](../api/user-delta.md), [групп](../api/group-delta.md), [приложений](../api/application-delta.md) и [субъектов-служб](../api/serviceprincipal-delta.md). Каждый производный тип поддерживает фильтрацию по **id**. Дополнительные сведения о разностных запросах см. в статье [Отслеживание изменений данных Microsoft Graph с помощью разностного запроса](/graph/delta-query-overview).|

## <a name="properties"></a>Свойства

| Свойство   | Тип |Описание|
|:---------------|:--------|:----------|
|id|String|Уникальный идентификатор объекта. Например, 12345678-9abc-def0-1234-56789abcde. Значение свойства **идентификатор** оформлено часто, но не всегда в виде GUID; необходимо считать его непрозрачным идентификатором и не полагаться на то, что он является GUID. Ключевое. Не допускается значение NULL. Только для чтения.|

## <a name="relationships"></a>Связи

Отсутствуют.


## <a name="json-representation"></a>Представление в формате JSON

Ниже представлено описание ресурса в формате JSON.

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.directoryObject",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false
      }
    }
  ]
}-->

```json
{
  "id": "string (identifier)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "directoryObject resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

