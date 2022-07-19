---
title: Тип ресурса ediscoveryHoldPolicy
description: '*Тип ресурса ediscoveryHoldPolicy'
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 46207724e8f8b2b23dc3d42543de8af67390ce87
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837564"
---
# <a name="ediscoveryholdpolicy-resource-type"></a>Тип ресурса ediscoveryHoldPolicy

Пространство имен: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет политику удержания по юридическим причинам. Удержания по юридическим причинам связаны с делом обнаружения электронных данных. Удержания по юридическим причинам не следует путать с удержаниями, которые используются для управления политиками хранения для содержимого Microsoft 365. Удержания по юридическим причинам обнаружения электронных данных предназначены для хранения содержимого на неограниченное время для судебного разбирательства, внутренних расследований и других юридических действий, в которых содержимое должно быть защищено от удаления. Дополнительные сведения см. в разделе ["Управление удержаниями в службе обнаружения электронных данных (цен. категория "Премиум")](/microsoft-365/compliance/managing-holds)

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление объектов ediscoveryHoldPolicies](../api/security-ediscoverycase-list-legalholds.md)|[Коллекция microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Получение списка объектов [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) и их свойств.|
|[Создание ediscoveryHoldPolicy](../api/security-ediscoverycase-post-legalholds.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Создайте объект [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Получение ediscoveryHoldPolicy](../api/security-ediscoveryholdpolicy-get.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Чтение свойств и связей объекта [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Обновление ediscoveryHoldPolicy](../api/security-ediscoveryholdpolicy-update.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|Обновление свойств объекта [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Удаление ediscoveryHoldPolicy](../api/security-ediscoverycase-delete-legalholds.md)|Нет|Удаление объекта [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) .|
|[Перечисление siteSources](../api/security-ediscoverycustodian-list-sitesources.md)|[Коллекция microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Получите ресурсы siteSource из свойства навигации siteSources.|
|[Создание siteSource](../api/security-ediscoveryholdpolicy-post-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Создайте объект siteSource.|
|[Перечисление userSources](../api/security-ediscoverycustodian-list-usersources.md)|[Коллекция microsoft.graph.security.userSource](../resources/security-usersource.md)|Получение ресурсов userSource из свойства навигации userSources.|
|[Создание userSource](../api/security-ediscoveryholdpolicy-post-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md)|Создайте объект userSource.|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|contentQuery|Строка|KQL-запрос, указывающий содержимое, которое должно храниться в указанных расположениях. Дополнительные сведения см. в статьях о [запросах по ключевым словам и условиях поиска для поиска контента и обнаружения электронных данных](/microsoft-365/compliance/keyword-queries-and-search-conditions).  Чтобы хранить все содержимое в указанных расположениях, оставьте **contentQuery пустым** . |
|createdBy|[identitySet](../resources/identityset.md)|Пользователь, создавший удержание по юридическим причинам. |
|createdDateTime|DateTimeOffset|Дата и время создания удержания по юридическим причинам. |
|description|String| Описание удержания по юридическим причинам. |
|displayName|Строка| Отображаемое имя удержания по юридическим причинам. |
|ошибки|Коллекция строк|Выводит список ошибок, которые произошли при размещении удержания. |
|id|String|Идентификатор дела обнаружения электронных данных. Только для чтения. Наследуется от [сущности](../resources/entity.md). |
|isEnabled|Boolean|Указывает, включено ли удержание и активно ли содержимое. |
|lastModifiedBy|[identitySet](../resources/identityset.md)|Пользователь, который последним изменил удержание по юридическим причинам.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения удержания по юридическим причинам. |
|status|microsoft.graph.security.policyStatus|Состояние удержания по юридическим причинам. Возможные значения: `Pending`, `Error`, `Success`.|

### <a name="policystatus-values"></a>Значения policyStatus

|Member|Описание|
|:---|-----------|
|Pending| Выполняется процесс распределения удержания. |
|Error| При применении удержания произошла ошибка. |
|Успешно| Удержание успешно применено и содержит указанное содержимое. |

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|siteSources|[Коллекция microsoft.graph.security.siteSource](../resources/security-sitesource.md)|Источники данных, которые представляют сайты SharePoint.|
|userSources|[Коллекция microsoft.graph.security.userSource](../resources/security-usersource.md)|Источники данных, которые представляют почтовые ящики Exchange.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryHoldPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryHoldPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "isEnabled": "Boolean",
  "contentQuery": "String",
  "errors": [
    "String"
  ]
}
```

