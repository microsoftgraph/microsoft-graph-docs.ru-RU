---
title: тип ресурса userFlowLanguagePage
description: Используются языковые страницы потока пользователей, которые определяют, какие строки будут показаны пользователям во время пользовательского путешествия, настроенного с помощью пользовательских потоков.
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7a52d1dce81bc24809d788e8d28ef869b84c4704
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629520"
---
# <a name="userflowlanguagepage-resource-type"></a>тип ресурса userFlowLanguagePage

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Используются языковые страницы потока пользователей, которые определяют, какие строки будут показаны пользователям во время пользовательского путешествия, настроенного с помощью пользовательских потоков. Эти языковые страницы включают как языковые переводы по умолчанию, предоставляемые Корпорацией Майкрософт, так и настраиваемые страницы, которые можно создать для настройки языковых переводов.

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
