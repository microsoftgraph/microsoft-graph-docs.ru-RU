---
title: тип ресурса accessPackageResourceEnvironment
description: Среда ресурсов пакета доступа является ссылкой на среду геолокации, в которой находится ресурс.
author: hanki-microsoft
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 0a1d9362371b9a479d12ba6613e49854283bd610
ms.sourcegitcommit: fd609cb401ff862c3f5c21847bac9af967c6bf82
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/31/2021
ms.locfileid: "61651198"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>тип ресурса accessPackageResourceEnvironment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-overview.md)среда ресурсов пакета доступа является ссылкой на среду геолокации, в которой находится ресурс. Эта среда автоматически предоставляется в рамках управления правами Azure AD. API применим только к сайтам Multi-Geo SharePoint Online.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessPackageResourceEnvironments](../api/entitlementmanagement-list-accesspackageresourceenvironment.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection|Извлечение списка [объектов accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Получите accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Ознакомьтесь с свойствами и отношениями объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|Сведения о подключении среды, используемой для подключения к ресурсу. |
|createdBy|String|Отображает имя пользователя, создав этот объект.|
|createdDateTime|DateTimeOffset|Дата и время создания этого объекта. <br>Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|description|Строка|Описание этого объекта.|
|displayName|Строка|Отображает имя этого объекта.|
|id|Строка|Уникальный идентификатор объекта, назначенного системой.|
|isDefaultEnvironment|Boolean|Определяет, является ли это среда по умолчанию или нет. Он установлен для `true` всех систем статического происхождения, таких как группы Azure AD и Приложения Azure AD.|
|modifiedBy|Строка|Отображает имя сущности, которая в последний раз меняла этот объект.|
|modifiedDateTime|DateTimeOffset|Дата и время последнего изменения этого объекта. <br>Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|OriginId|Строка|Уникальный идентификатор этой среды в системе происхождения.|
|originSystem|Строка|Тип ресурса в системе происхождения, то есть `SharePointOnline` . Requires `$filter` ( `eq` ).|

## <a name="relationships"></a>Отношения
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackageResources|[коллекция accessPackageResource](../resources/accesspackageresource.md)|Только для чтения. Обязательный.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.accessPackageResourceEnvironment",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "originSystem": "String",
  "originId": "String",
  "isDefaultEnvironment": "Boolean",
  "connectionInfo": {
    "@odata.type": "microsoft.graph.connectionInfo"
  },
  "createdBy": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedBy": "String",
  "modifiedDateTime": "String (timestamp)"
}
```
