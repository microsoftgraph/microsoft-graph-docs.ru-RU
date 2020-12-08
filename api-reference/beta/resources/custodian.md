---
title: Тип ресурса хранитель
description: В контексте обнаружения электронных данных представляет пользователя и все свои цифровые ресурсы, такие как электронная почта и документы.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: a2e22f711eaec4cd68cc5026e36b900d5284e71a
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597831"
---
# <a name="custodian-resource-type"></a>Тип ресурса хранитель

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В контексте обнаружения электронных данных представляет пользователя и все свои цифровые ресурсы, такие как электронная почта и документы.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список custodians](../api/ediscoverycase-list-custodians.md)|Коллекция [хранитель](../resources/custodian.md)|Получение списка объектов **хранитель** и их свойств.|
|[Создание хранитель](../api/ediscoverycase-post-custodians.md)|[Хранитель](../resources/custodian.md)|Создание нового объекта **хранитель** .|
|[Получение хранитель](../api/custodian-get.md)|[Хранитель](../resources/custodian.md)|Чтение свойств и связей объекта **хранитель** .|
|[Обновление хранитель](../api/custodian-update.md)|[Хранитель](../resources/custodian.md)|Обновление свойств объекта **хранитель** .|
|[удаления](../api/custodian-release.md)|Нет|Освобождение хранитель от случая.|
|[отключить](../api/custodian-activate.md)|Нет|Повторно активируйте хранитель, выпущенные из случая, и сделайте их частью этого случая.|
|[Список Ситесаурцес](../api/custodian-list-sitesources.md)|Коллекция [ситесаурце](../resources/sitesource.md)|Получение ресурсов **ситесаурце** из свойства навигации **ситесаурцес** .|
|[Создание Ситесаурцес](../api/custodian-post-sitesources.md)|[ситесаурце](../resources/sitesource.md)|Создание нового объекта **ситесаурце** .|
|[Список Унифиедграупсаурцес](../api/custodian-list-unifiedgroupsources.md)|Коллекция [унифиедграупсаурце](../resources/unifiedgroupsource.md)|Получение ресурсов **унифиедграупсаурце** из свойства навигации **унифиедграупсаурцес** .|
|[Создание Унифиедграупсаурцес](../api/custodian-post-unifiedgroupsources.md)|[унифиедграупсаурце](../resources/unifiedgroupsource.md)|Создание нового объекта **унифиедграупсаурце** .|
|[Список Усерсаурцес](../api/custodian-list-usersources.md)|Коллекция [усерсаурце](../resources/usersource.md)|Получение ресурсов **усерсаурце** из свойства навигации **усерсаурцес** .|
|[Создание Усерсаурцес](../api/custodian-post-usersources.md)|[усерсаурце](../resources/usersource.md)|Создание нового объекта **усерсаурце** .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|аккновледжеддатетиме|DateTimeOffset|Дата и время, когда хранитель подтвердил уведомление об удержании.|
|апплихолдтосаурцес|Логический|Определяет, были ли источники хранитель сохранены во время создания.|
|createdDateTime|DateTimeOffset|Дата и время добавления хранитель к обращению.|
|displayName|String|Отображаемое имя хранитель.|
|email|String|Адрес электронной почты хранитель.|
|id|String|Идентификатор хранитель в указанном случае. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта хранитель|
|релеаседдатетиме|DateTimeOffset|Дата и время, когда хранитель был выпущен из дела.|
|status|кустодианстатус|Состояние хранитель. Возможные значения: `active`, `released`.|

### <a name="custodianstatus-values"></a>значения Кустодианстатус

|Member|Описание|
|:----|-----------|
|ASP|Хранитель — это активная часть этого случая. |
|снят|Хранитель выпущен из этого случая.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|ситесаурцес|Коллекция [ситесаурце](../resources/sitesource.md)|Объект источника данных для сайтов SharePoint, связанных с хранитель.|
|унифиедграупсаурцес|Коллекция [унифиедграупсаурце](../resources/unifiedgroupsource.md)|Сущность источника данных для групп, связанных с хранитель.|
|усерсаурцес|Коллекция [усерсаурце](../resources/usersource.md)|Сущность источника данных для объекта хранитель. Это контейнер для почтового ящика хранитель и сайта OneDrive для бизнеса.|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.custodian",
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
