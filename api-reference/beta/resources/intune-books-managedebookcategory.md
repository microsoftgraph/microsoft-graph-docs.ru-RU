---
title: Тип ресурса managedEBookCategory
description: Содержит свойства для одной категории Intune электронная книга.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b415554d47c33f06a917c10327dad983db762578
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894189"
---
# <a name="managedebookcategory-resource-type"></a>Тип ресурса managedEBookCategory

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для одной категории Intune электронная книга.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список managedEBookCategories](../api/intune-books-managedebookcategory-list.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md) коллекции|Свойства списка и связей объектов [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .|
|[Получение managedEBookCategory](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Чтение свойства и связи объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .|
|[Создание managedEBookCategory](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Создание нового объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .|
|[Удаление managedEBookCategory](../api/intune-books-managedebookcategory-delete.md)|Нет|Удаляет [managedEBookCategory](../resources/intune-books-managedebookcategory.md).|
|[Обновление managedEBookCategory](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Обновление свойства объекта [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|Строка|Имя категории электронная книга.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения ManagedEBookCategory.|

## <a name="relationships"></a>Связи
Нет
## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```





