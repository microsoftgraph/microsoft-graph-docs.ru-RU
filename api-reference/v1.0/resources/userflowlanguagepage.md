---
title: тип ресурса userFlowLanguagePage
description: Определяет строки, которые показаны пользователям во время потока пользователей.
author: jkdouglas
ms.localizationpriority: medium
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 3c8367b29b857d7b1bce9dc5815ede5b74f5c025
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136315"
---
# <a name="userflowlanguagepage-resource-type"></a>тип ресурса userFlowLanguagePage

Пространство имен: microsoft.graph

Определяет языковые страницы потока пользователей, которые показаны пользователям во время потока пользователей. Эти языковые страницы включают как языковые переводы по умолчанию, предоставляемые Корпорацией Майкрософт, так и настраиваемые страницы, которые можно создать для настройки языковых переводов.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get userFlowLanguagePage](../api/userflowlanguagepage-get.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Извлечение значений объекта по умолчанию или [пользовательского пользователяFlowLanguagePage.](../resources/userflowlanguagepage.md)|
|[Обновление userFlowLanguagePage](../api/userflowlanguagepage-put.md)|[userFlowLanguagePage](../resources/userflowlanguagepage.md)|Обновление значений в настраиваемом [объекте userFlowLanguagePage.](../resources/userflowlanguagepage.md)|
|[Удаление userFlowLanguagePage](../api/userflowlanguagepage-delete.md)|Нет|Удаляет значения из пользовательского [объекта userFlowLanguagePage.](../resources/userflowlanguagepage.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор страницы userFlowLanguage.|

## <a name="relationships"></a>Отношения

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userFlowLanguagePage",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.userFlowLanguagePage",
  "id": "String (identifier)"
}
```
