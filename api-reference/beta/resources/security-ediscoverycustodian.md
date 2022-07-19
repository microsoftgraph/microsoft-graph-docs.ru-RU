---
title: Тип ресурса ediscoveryCustodian
description: В контексте обнаружения электронных данных представляет пользователя и все его цифровые ресурсы, такие как электронная почта и документы.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b9edba3e4521177e26b3b13d409c4a6c7c1ea025
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837550"
---
# <a name="ediscoverycustodian-resource-type"></a>Тип ресурса ediscoveryCustodian

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В контексте обнаружения электронных данных представляет пользователя и все его цифровые ресурсы, такие как электронная почта и документы.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление ediscoveryCustodians](../api/security-ediscoverycase-list-custodians.md)|[Коллекция microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Получение списка объектов [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) и их свойств.|
|[Создание объекта ediscoveryCustodian](../api/security-ediscoverycase-post-custodians.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Создайте объект [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) .|
|[Get ediscoveryCustodian](../api/security-ediscoverycustodian-get.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|Чтение свойств и связей объекта [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) .|
|[updateIndex](../api/security-ediscoverycustodian-updateindex.md)|Активирует indexOperation, чтобы сделать хранителя и связанные источники доступны для поиска.|
|[Активировать](../api/security-ediscoverycustodian-activate.md)|Нет|Повторно активируйте хранителя из дела.|
|[Выпуска](../api/security-ediscoverycustodian-release.md)|Нет|Освобождение хранителя из дела.|
|[applyHold](../api/security-ediscoverycustodian-applyhold.md)|Нет|Запустите процесс применения удержания к хранителям обнаружения электронных данных.|
|[removeHold](../api/security-ediscoverycustodian-removehold.md)|Нет|Запустите процесс удаления удержания у хранителей обнаружения электронных данных.|
|[Перечисление ediscoveryIndexOperation](../api/security-ediscoverycustodian-list-lastindexoperation.md)|[Коллекция microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Получение списка [ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md) , связанного с [ediscoveryCustodian](../resources/security-ediscoverycustodian.md).|
|[Перечисление siteSources](../api/security-ediscoverycustodian-list-sitesources.md)|[Коллекция microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Получите ресурсы siteSource из свойства навигации siteSources.|
|[Создание siteSource](../api/security-ediscoverycustodian-post-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Создайте объект [siteSource](../resources/security-sitesource.md) , связанный с [хранителями обнаружения электронных данных](../resources/security-ediscoverycustodian.md).|
|[Перечисление unifiedGroupSources](../api/security-ediscoverycustodian-list-unifiedgroupsources.md)|[Коллекция microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md)|Получите ресурсы unifiedGroupSource из свойства навигации unifiedGroupSources.|
|[Создание unifiedGroupSource](../api/security-ediscoverycustodian-post-unifiedgroupsources.md)|[microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md)|Создайте новый [объект unifiedGroupSource](../resources/security-unifiedgroupsource.md) , связанный с хранителям [обнаружения электронных данных](../resources/security-ediscoverycustodian.md).|
|[Перечисление userSources](../api/security-ediscoverycustodian-list-usersources.md)|[Коллекция microsoft.graph.security.userSource](../resources/security-usersource.md)|Получение ресурсов userSource из свойства навигации userSources.|
|[Создание userSource](../api/security-ediscoverycustodian-post-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md)|Создайте объект [userSource](../resources/security-usersource.md) , связанный с хранителями [обнаружения электронных данных](../resources/security-ediscoverycustodian.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|Дата и время подтверждения уведомления о удержании хранителя.|
|createdDateTime|DateTimeOffset|Дата и время добавления хранителя в дело.|
|displayName|String|Отображаемое имя хранителя.|
|email|String|Email адрес хранителя.|
|id|String|Идентификатор хранителя в указанном случае. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта хранителя|
|releasedDateTime|DateTimeOffset|Дата и время освобождения хранителя из дела.|
|status|microsoft.graph.security.dataSourceContainerStatus|Состояние хранителя. Возможные значения: `active`, `released`.|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|Состояние удержания хранителя. Возможные значения: `notApplied`, , `applied`, `applying`, `removing``partial`|

### <a name="custodianstatus-values"></a>Значения custodianStatus

|Имя|Описание|
|:----|-----------|
|Активных|Хранителя является активной частью дела. |
|Выпущен|Хранитель освобожден из дела.|

### <a name="custodianholdstatus-values"></a>Значения custodianHoldStatus

|Имя|Описание|
|:----|-----------|
|notApplied|Хранитель не находится на удержании (все источники в нем не находятся на удержании).|
|Применяется|Хранитель находится на удержании (все источники находятся на удержании).|
|Применение|Хранителя применяет состояние удержания (активируется операция applyHold).|
|Удаление|Хранителя удаляет состояние удержания (операция removeHold активируется).|
|Частичное|Хранителя находится в смешанном состоянии, где некоторые источники находятся на удержании, а некоторые не находятся в состоянии удержания или ошибки.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|lastIndexOperation|[microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|Сущность операции, представляющая последнее индексирование для хранителя.|
|siteSources|[Коллекция microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Сущность источника данных для сайтов SharePoint, связанных с хранителями.|
|unifiedGroupSources|[Коллекция microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md)|Сущность источника данных для групп, связанных с хранителями.|
|userSources|[Коллекция microsoft.graph.security.userSource](../resources/security-usersource.md)|Сущность источника данных для хранителя. Это контейнер для почтового ящика хранителя и OneDrive для бизнеса сайта.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCustodian",
  "baseType": "microsoft.graph.security.dataSourceContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCustodian",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "email": "String",
  "acknowledgedDateTime": "String (timestamp)"
}
```

