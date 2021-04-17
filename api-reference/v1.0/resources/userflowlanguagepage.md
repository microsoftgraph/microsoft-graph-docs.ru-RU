---
title: тип ресурса userFlowLanguagePage
description: Определяет строки, которые показаны пользователям во время потока пользователей.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: b3f3610607bfeef5f3e47a110c2491b635555494
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/17/2021
ms.locfileid: "51883307"
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
|id|Строка|Идентификатор страницы userFlowLanguage.|

## <a name="relationships"></a>Связи

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
