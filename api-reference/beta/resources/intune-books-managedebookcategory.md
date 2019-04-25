---
title: Тип ресурса Манажедебуккатегори
description: Содержит свойства для одной категории электронной книги Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef3d0d621394af0cfe949031d79ff374ba0491b8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548294"
---
# <a name="managedebookcategory-resource-type"></a>Тип ресурса Манажедебуккатегори

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для одной категории электронной книги Intune.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Манажедебуккатегориес](../api/intune-books-managedebookcategory-list.md)|Коллекция [манажедебуккатегори](../resources/intune-books-managedebookcategory.md)|Список свойств и связей объектов [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .|
|[Получение Манажедебуккатегори](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Чтение свойств и связей объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .|
|[Создание Манажедебуккатегори](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Создание нового объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .|
|[Удаление Манажедебуккатегори](../api/intune-books-managedebookcategory-delete.md)|Нет|Удаляет объект [манажедебуккатегори](../resources/intune-books-managedebookcategory.md).|
|[Обновление Манажедебуккатегори](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md);|Обновление свойств объекта [манажедебуккатегори](../resources/intune-books-managedebookcategory.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|displayName|String|Имя категории электронной книги.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения Манажедебуккатегори.|

## <a name="relationships"></a>Отношения
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





