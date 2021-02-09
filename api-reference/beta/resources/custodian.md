---
title: Тип ресурса custodian
description: В контексте eDiscovery представляет пользователя и все его цифровые активы, такие как электронная почта и документы.
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 6c6b2befbb4066b851e38e6e17fd8be5aa59b031
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157696"
---
# <a name="custodian-resource-type"></a>Тип ресурса custodian

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В контексте eDiscovery представляет пользователя и все его цифровые активы, такие как электронная почта и документы.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список хранителей](../api/ediscoverycase-list-custodians.md)|[коллекция custodian](../resources/custodian.md)|Получите список объектов **хранителя** и их свойств.|
|[Создание хранителя](../api/ediscoverycase-post-custodians.md)|[custodian](../resources/custodian.md)|Создание объекта **хранителя.**|
|[Получить хранителя](../api/custodian-get.md)|[custodian](../resources/custodian.md)|Чтение свойств и связей объекта **хранителя.**|
|[Обновление хранителя](../api/custodian-update.md)|[custodian](../resources/custodian.md)|Обновление свойств объекта **custodian.**|
|[release](../api/custodian-release.md)|Нет|Освобождение хранителя из дела.|
|[activate](../api/custodian-activate.md)|Нет|Повторно активировать хранителя, освобожденного из дела, и снова сделать его частью дела.|
|[Список siteSources](../api/custodian-list-sitesources.md)|[Коллекция siteSource](../resources/sitesource.md)|Получите ресурсы **siteSource** из свойства навигации **siteSources.**|
|[Создание siteSources](../api/custodian-post-sitesources.md)|[siteSource](../resources/sitesource.md)|Создание объекта **siteSource.**|
|[Список unifiedGroupSources](../api/custodian-list-unifiedgroupsources.md)|[Коллекция unifiedGroupSource](../resources/unifiedgroupsource.md)|Получите ресурсы **unifiedGroupSource из** свойства навигации **unifiedGroupSources.**|
|[Создание unifiedGroupSources](../api/custodian-post-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|Создание объекта **unifiedGroupSource.**|
|[Список userSources](../api/custodian-list-usersources.md)|[Коллекция userSource](../resources/usersource.md)|Получите ресурсы **userSource** из свойства **навигации userSources.**|
|[Создание userSources](../api/custodian-post-usersources.md)|[userSource](../resources/usersource.md)|Создание объекта **userSource.**|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|Дата и время, когда хранител подтвердил уведомление об удержании.|
|applyHoldToSources|Boolean|Определяет, были ли источники хранителя помещены на удержание во время создания.|
|createdDateTime|DateTimeOffset|Дата и время, когда хранители были добавлены в дело.|
|displayName|String|Отображаемого имени хранителя.|
|email|String|Адрес электронной почты хранителя.|
|id|String|ИД хранителя в указанном случае. Только для чтения.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения объекта хранителя|
|releasedDateTime|DateTimeOffset|Дата и время освобождения хранителя из дела.|
|status|custodianStatus|Состояние хранителя. Возможные значения: `active`, `released`.|

### <a name="custodianstatus-values"></a>значения custodianStatus

|Member|Описание|
|:----|-----------|
|active|Хранителя является активной частью дела. |
|released|Хранители освобождены из дела.|

## <a name="relationships"></a>Связи

|Связь|Тип|Описание|
|:---|:---|:---|
|siteSources|[Коллекция siteSource](../resources/sitesource.md)|Объект источника данных для сайтов SharePoint, связанных с хранителями.|
|unifiedGroupSources|[Коллекция unifiedGroupSource](../resources/unifiedgroupsource.md)|Объект источника данных для групп, связанных с хранителями.|
|userSources|[Коллекция userSource](../resources/usersource.md)|Объект источника данных для хранителя. Это контейнер для почтового ящика хранителя и сайта OneDrive для бизнеса.|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>Представление JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
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
