---
title: Тип ресурса userFlowLanguagePage
description: Используемые страницы языка пользовательского потока определяют, какие строки пользователи будут показывать во время пользовательского пути, настроенного с помощью пользовательских потоков.
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d6a6bd597fb274d8fdb8150be0a2c5e085949156
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/17/2020
ms.locfileid: "49706374"
---
# <a name="userflowlanguagepage-resource-type"></a>Тип ресурса userFlowLanguagePage

Пространство имен: microsoft.graph

Используемые страницы языка пользовательского потока определяют, какие строки пользователи будут показывать во время пользовательского пути, настроенного с помощью пользовательских потоков. Эти языковые страницы включают как переводы языка по умолчанию, предоставляемые корпорацией Майкрософт, так и настраиваемые страницы, которые можно создать для настройки перевода языков.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get userFlowLanguagePage](../api/userflowlanguagepage-get.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Извлечение значений объекта [userFlowLanguagePage](../resources/userflowlanguagepage.md) по умолчанию или пользовательского объекта.|
|[Обновление userFlowLanguagePage](../api/userflowlanguagepage-put.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Обновление значений в настраиваемом [объекте userFlowLanguagePage.](../resources/userflowlanguagepage.md)|
|[Удаление userFlowLanguagePage](../api/userflowlanguagepage-delete.md)|Нет|Удаляет значения из пользовательского [объекта userFlowLanguagePage.](../resources/userflowlanguagepage.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор страницы userFlowLanguage.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "baseType": "",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
