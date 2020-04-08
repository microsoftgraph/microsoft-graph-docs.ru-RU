---
title: Тип ресурса Директорисеттингтемплате
description: Шаблоны параметров каталога представляют системные параметры, доступные для клиента.
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 03803fddb12401e8d04318e8f4e7d7c63029b709
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181527"
---
# <a name="directorysettingtemplate-resource-type"></a>Тип ресурса Директорисеттингтемплате

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Шаблоны параметров каталога представляют системные параметры, доступные для клиента. [Параметры каталога](directorysetting.md) могут быть созданы на основе доступных директорисеттингтемплатес, и значения, заданные по умолчанию, изменяются. Шаблоны параметров каталога невозможно создать, обновить или удалить. Эти параметры могут представлять параметры на уровне клиента или конкретные параметры сущности.  В настоящее время доступны только шаблоны для групп Office, а также параметры, например, могут ли пользователи создавать группы или приглашать гостей извне организации для становиться членами группы.

> **Note**: версия/Beta типа ресурса директорисеттингтемплате применяется только к группам. Версия/v1.0 переименована в groupSettingTemplate.

## <a name="methods"></a>Методы

| Метод           | Возвращаемый тип    |Описание|
|:---------------|:--------|:----------|
|[Получение Директорисеттингтемплате](../api/directorysettingtemplate-get.md) | [directorySettingTemplate](directorysettingtemplate.md) |Чтение определенных свойств одного из системных объектов Директорисеттингтемплате, определенных системой.|
|[Список Директорисеттингтемплате](../api/directorysettingtemplate-list.md) | [Коллекция Директорисеттингтемплате](directorysettingtemplate.md) |Перечисление всех объектов Директорисеттингтемплате, определенных системой.|

## <a name="properties"></a>Свойства
| Свойство     | Тип   |Описание|
|:---------------|:--------|:----------|
|description|string|Описание шаблона. Только для чтения.|
|displayName|string|Отображаемое имя шаблона. Только для чтения. |
|id|строка| Уникальный идентификатор шаблона. Только для чтения.|
|values|Коллекция [сеттингтемплатевалуе](settingtemplatevalue.md)| Коллекция Settingtemplatevalue, в которой перечислены набор доступных параметров, значения по умолчанию и типы, которые составляют этот шаблон.  Только для чтения. |

## <a name="relationships"></a>Отношения
Нет


## <a name="json-representation"></a>Представление JSON

Ниже представлено описание ресурса в формате JSON.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.directorySettingTemplate"
}-->

```json
{
  "description": "string",
  "displayName": "string",
  "id": "string (identifier)",
  "values": [{"@odata.type": "microsoft.graph.settingTemplateValue"}]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directorySettingTemplate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
