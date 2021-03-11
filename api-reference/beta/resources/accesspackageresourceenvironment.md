---
title: тип ресурса accessPackageResourceEnvironment
description: Среда ресурсов пакета доступа является ссылкой на среду геолокации, в которой находится ресурс.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 09bd318036874bb52bfab0ed522a2948cbe83233
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722202"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>тип ресурса accessPackageResourceEnvironment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [Azure AD Entitlement Management](entitlementmanagement-root.md)среда ресурсов пакета доступа является ссылкой на среду геолокации, в которой находится ресурс. Эта среда автоматически предоставляется в рамках управления правами Azure AD. API применим только к сайтам Multi-Geo SharePoint Online.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md) collection|Извлечение списка [объектов accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Получите accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Ознакомьтесь с свойствами и отношениями объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|Сведения о подключении среды, используемой для подключения к ресурсу. |
|createdBy|String|Отображает имя пользователя, создав этот объект.|
|createdDateTime|DateTimeOffset|Дата и время создания этого объекта. <br>Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|description|String|Описание этого *объекта accessPackageResourceEnvironment.*|
|displayName|String|Отображает имя этого объекта.|
|id|String|Уникальный идентификатор объекта, назначенного системой.|
|isDefaultEnvironment|Boolean|Определяет, является ли это среда по умолчанию или нет. Он установлен для `true` всех систем статического происхождения, таких как группы Azure AD и Приложения Azure AD.|
|modifiedBy|String|Отображает имя сущности, которая в последний раз меняла этот объект.|
|modifiedDateTime|DateTimeOffset|Дата и время последнего изменения этого объекта. <br>Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`. |
|OriginId|String|Уникальный идентификатор этой среды в системе происхождения.|
|originSystem|String|Тип ресурса в системе происхождения, например `SharePointOnline` . Поддерживает `$filter`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackageResources|[коллекция accessPackageResource](../resources/accesspackageresource.md)|Только для чтения. Обязательный атрибут.|

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
