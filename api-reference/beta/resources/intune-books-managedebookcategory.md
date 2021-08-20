---
title: тип ресурсов managedEBookCategory
description: Содержит свойства для одной категории электронных книг Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6b877365fb12bf1baede2248b4f52ba6109643d841adfb239d358aaefc4d1fed
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213279"
---
# <a name="managedebookcategory-resource-type"></a>тип ресурсов managedEBookCategory

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для одной категории электронных книг Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список управляемыхEBookCategories](../api/intune-books-managedebookcategory-list.md)|[коллекция managedEBookCategory](../resources/intune-books-managedebookcategory.md)|Список свойств и связей управляемых [объектовEBookCategory.](../resources/intune-books-managedebookcategory.md)|
|[УправлениеEBookCategory](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Чтение свойств и связей объекта [managedEBookCategory.](../resources/intune-books-managedebookcategory.md)|
|[Создание managedEBookCategory](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Создайте новый [объект managedEBookCategory.](../resources/intune-books-managedebookcategory.md)|
|[Удаление управляемогоEBookCategory](../api/intune-books-managedebookcategory-delete.md)|Нет|Удаляет [управляемыйEBookCategory](../resources/intune-books-managedebookcategory.md).|
|[Обновление managedEBookCategory](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Обновление свойств объекта [managedEBookCategory.](../resources/intune-books-managedebookcategory.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|Строка|Имя категории электронных книг.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения managedEBookCategory.|

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




