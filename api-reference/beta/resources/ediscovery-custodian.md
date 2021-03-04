---
title: тип ресурса хранителя
description: В контексте eDiscovery представляет пользователя и все его цифровые активы, такие как электронная почта и документы.
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 0d71542b796f5256f21e19a886533e3a88e1d7ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447554"
---
# <a name="custodian-resource-type"></a>тип ресурса хранителя

Пространство имен: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В контексте eDiscovery представляет пользователя и все его цифровые активы, такие как электронная почта и документы.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Хранители списка](../api/ediscovery-case-list-custodians.md)|[коллекция microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|Получите список **объектов-хранителя** и их свойств.|
|[Создание хранителя](../api/ediscovery-case-post-custodians.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|Создайте новый **объект хранителя.**|
|[Получить хранителя](../api/ediscovery-custodian-get.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|Ознакомьтесь с свойствами и отношениями **объекта-хранителя.**|
|[Хранители обновлений](../api/ediscovery-custodian-update.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|Обновление свойств **объекта-хранителя.**|
|[выпуск](../api/ediscovery-custodian-release.md)|Нет|Освобождение хранителя из дела.|
|[активировать](../api/ediscovery-custodian-activate.md)|Нет|Повторно активировать хранителя, который был освобожден из дела, и снова сделать их частью дела.|
|[List siteSources](../api/ediscovery-custodian-list-sitesources.md)|[коллекция microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Получите **ресурсы siteSource,** связанные с хранителями.|
|[Создание siteSources](../api/ediscovery-custodian-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Создание нового **объекта siteSource.**|
|[Список унифицированныхGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)|[коллекция microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Получите список ресурсов **unifiedGroupSource,** связанных с хранителями.|
|[Создание unifiedGroupSources](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Создание нового **объекта unifiedGroupSource.**|
|[Список userSources](../api/ediscovery-custodian-list-usersources.md)|[коллекция microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Получите список ресурсов **userSource,** связанных с хранителями.|
|[Создание userSources](../api/ediscovery-custodian-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Создание нового **объекта userSource.**|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|Дата и время, когда хранитель подтвердил уведомление о удержании.|
|applyHoldToSources|Boolean|Определяет, были ли приодержится источники хранителя во время создания.|
|createdDateTime|DateTimeOffset|Дата и время, когда хранитель был добавлен в дело.|
|displayName|String|Отображение имени хранителя.|
|email|String|Адрес электронной почты хранителя.|
|id|String|ID для хранителя в указанном случае. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта хранителя|
|releasedDateTime|DateTimeOffset|Дата и время освобождения хранителя из дела.|
|status|microsoft.graph.ediscovery.custodianStatus|Состояние хранителя. Возможные значения: `active`, `released`.|

### <a name="custodianstatus-values"></a>значения custodianStatus

|Member|Описание|
|:----|-----------|
|active|Хранитель является активной частью дела. |
|выпущено|Хранитель освобожден из дела.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|siteSources|[коллекция microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|Объект источника данных для сайтов SharePoint, связанных с хранителями.|
|unifiedGroupSources|[коллекция microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|Объект источника данных для групп, связанных с хранителями.|
|userSources|[коллекция microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|Объект источника данных для хранителя. Это контейнер для почтового ящика хранителя и сайта OneDrive для бизнеса.|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.custodian",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.custodian",
  "email": "String",
  "applyHoldToSources": "Boolean",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "acknowledgedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String"
}
```
