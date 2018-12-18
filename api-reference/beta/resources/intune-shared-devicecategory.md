---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: tfitzmac
ms.openlocfilehash: 4416dc1557cdae38313aa8aa1e73cda82d764e9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359544"
---
# <a name="devicecategory-resource-type"></a>Тип ресурса deviceCategory

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Категории устройств предоставляют способ организации устройство. С помощью категории устройств, компании администраторы могут определить уникальный категорий, относящиеся к своей компании.Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceCategory](../api/intune-shared-devicecategory-list.md)|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Получение объекта deviceCategory](../api/intune-shared-devicecategory-get.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Создание объекта deviceCategory](../api/intune-shared-devicecategory-create.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Удаление объекта deviceCategory](../api/intune-shared-devicecategory-delete.md)|Нет|Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Обновление объекта deviceCategory](../api/intune-shared-devicecategory-update.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор категории устройства. Только для чтения.|
|**Адаптация новых сотрудников**|
|displayName|String|Отображаемое имя категории устройств.|
|описание|String|Необязательное описание категории устройств.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



