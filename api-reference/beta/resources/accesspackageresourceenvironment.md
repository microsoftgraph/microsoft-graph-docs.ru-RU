---
title: Тип ресурса accessPackageResourceEnvironment
description: Среда ресурсов пакета доступа — это ссылка на среду географического местонахождения, в которой расположен ресурс.
author: hanki-microsoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 814e77cb8122773bc425180c7e78a2794c9e0784
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137730"
---
# <a name="accesspackageresourceenvironment-resource-type"></a>Тип ресурса accessPackageResourceEnvironment

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

В [azure AD Entitlement Management](entitlementmanagement-root.md)среда ресурсов пакета доступа является ссылкой на среду географического местонахождения, в которой расположен ресурс. Эта среда автоматически предоставляется в рамках управления плитками Azure AD. API применим только к сайтам SharePoint Online с несколькими географическими режимами.

## <a name="methods"></a>Методы
|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Список accessPackageResourceEnvironments](../api/accesspackageresourceenvironment-list.md)|[Коллекция accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Получить список объектов [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|
|[Get accessPackageResourceEnvironment](../api/accesspackageresourceenvironment-get.md)|[accessPackageResourceEnvironment](../resources/accesspackageresourceenvironment.md)|Чтение свойств и связей объекта [accessPackageResourceEnvironment.](../resources/accesspackageresourceenvironment.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|connectionInfo|[connectionInfo](../resources/connectioninfo.md)|Сведения о подключении среды, используемой для подключения к ресурсу. |
|createdBy|String|Отображаемого имени пользователя, создав этот объект.|
|createdDateTime|DateTimeOffset|Дата и время создания объекта. <br>Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь 1 января 2014 г. в UTC — `'2014-01-01T00:00:00Z'` это .|
|description|Строка|Описание этого объекта *accessPackageResourceEnvironment.*|
|displayName|Строка|Отображаемого имени этого объекта.|
|id|Строка|Уникальный идентификатор объекта, присвоенный системе.|
|isDefaultEnvironment|Boolean|Определяет, является ли эта среда средой по умолчанию. Он установлен для всех систем статического источника, таких как группы `true` Azure AD и приложения Azure AD.|
|modifiedBy|Строка|Отображаемого имени объекта, который последним изменил этот объект.|
|modifiedDateTime|DateTimeOffset|Дата и время последнего изменения этого объекта. <br>Тип DateTimeOffset представляет сведения о дате и времени с использованием формата ISO 8601 и всегда указывает время в формате UTC. Например, полночь 1 января 2014 г. в UTC — `'2014-01-01T00:00:00Z'` это . |
|originId|Строка|Уникальный идентификатор этой среды в системе источника.|
|originSystem|Строка|Тип ресурса в системе источника, например `SharePointOnline` . Поддерживает `$filter`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|accessPackageResources|[Коллекция accessPackageResource](../resources/accesspackageresource.md)|Только для чтения. Обязательный элемент.|

## <a name="json-representation"></a>Представление JSON
Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.accessPackageResourceEnvironment",
  "baseType": "",
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
