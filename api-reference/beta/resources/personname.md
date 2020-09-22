---
title: Тип ресурса personName
description: Тип ресурса personName
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 1f1817e3d9868e47158453113f4781ebfc155f86
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/18/2020
ms.locfileid: "47997951"
---
# <a name="personname-resource-type"></a>Тип ресурса personName

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет сведения о расширенном имени, предоставленные пользователем или с которыми они связаны в своем [профиле](../resources/profile.md).

Наследуется от [итемфацет](../resources/itemfacet.md).

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список имен](../api/profile-list-names.md)|Коллекция [PersonName](../resources/personname.md)|Получение ресурсов personName из свойства навигации Names.|
|[Создание personName](../api/profile-post-names.md)|[personName](../resources/personname.md)|Создайте новый объект [PersonName](../resources/personname.md) на основе свойства навигации Names.|
|[Получение personName](../api/personname-get.md)|[personName](../resources/personname.md)|Чтение свойств и связей объекта [PersonName](../resources/personname.md) .|
|[Обновление personName](../api/personname-update.md)|[personName](../resources/personname.md)|Обновление свойств объекта [PersonName](../resources/personname.md) .|
|[Удаление personName](../api/personname-delete.md)|Нет|Удаляет объект [PersonName](../resources/personname.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|алловедаудиенцес|String|Аудитории, которые могут видеть значения, содержащиеся в сущности. Наследуется от [итемфацет](../resources/itemfacet.md). Возможные значения: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.|
|createdBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, создавшего сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|createdDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|displayName|String|Предоставляет упорядоченную визуализацию имени и фамилии в зависимости от языкового стандарта пользователя или устройства.|
|первыми|String|Имя пользователя.|
|id|String|Идентификатор, используемый для индивидуальной адресации объекта. Наследуется от [объекта](../resources/entity.md)|
|выводов|[инференцедата](../resources/inferencedata.md)|Содержит сведения о выводе, если объект создается или изменяется приложением. Наследуется от [итемфацет](../resources/itemfacet.md).|
|initials|String|Инициалы пользователя.|
|лангуажетаг|String|Содержит имя языка (EN-US, No-NetBIOS, en-AU), следуя формату IETF BCP47.   |
|Фамили|String|Фамилия пользователя.|
|lastModifiedBy|[identitySet](../resources/identityset.md)|Предоставляет идентификатор пользователя и/или приложения, которое последним изменил объект. Наследуется от [итемфацет](../resources/itemfacet.md).|
|lastModifiedDateTime|DateTimeOffset|Предоставляет значение dateTimeOffset для объекта, когда была создана сущность. Наследуется от [итемфацет](../resources/itemfacet.md).|
|маиден|String|Маиден имя пользователя. |
|назван|String|Отчество пользователя.|
|прозвищ|String|Псевдоним пользователя.|
|произношение|[йомиперсоннаме](../resources/yomipersonname.md)|Руководство по произношению имени пользователя.|
|source|[персондатасаурце](../resources/persondatasource.md)|Источник значений при синхронизации от другой службы. Наследуется от [итемфацет](../resources/itemfacet.md).|
|суффикс|String|Обозначения, используемые после имени пользователя (например, "доктор").  |
|title|String|Хонорификс используется для префикса имени пользователя (например, Dr, Sir, мадам, MRS).|

## <a name="relationships"></a>Связи
Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.personName",
  "baseType": "microsoft.graph.itemFacet",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.personName",
  "id": "e13f7a4d-303c-464f-a6af-80ea18eb74f3",
  "allowedAudiences": "organization",
  "inference": {
    "@odata.type": "microsoft.graph.inferenceData"
  },
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "source": {
    "@odata.type": "microsoft.graph.personDataSource"
  },
  "displayName": "Innocenty Popov",
  "first": "Innocenty",
  "initials": "IP",
  "last": "Popov",
  "languageTag": "en-US",
  "maiden": null,
  "middle": null,
  "nickname": "Kesha",
  "suffix": null,
  "title": null,
  "pronunciation": {
    "@odata.type": "microsoft.graph.yomiPersonName"
  }
}
```

