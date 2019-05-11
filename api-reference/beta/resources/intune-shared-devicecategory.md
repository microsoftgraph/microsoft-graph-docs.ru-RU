---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ff6c9d5bccb48338d88e0698ee58c0121cf49101
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939716"
---
# <a name="devicecategory-resource-type"></a>Тип ресурса deviceCategory

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Категории устройств обеспечивают способ организации устройств. С помощью категорий устройств Администраторы компании могут определять уникальные категории, которые имеют смысл в своей компании.Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceCategory](../api/intune-shared-devicecategory-list.md)|Коллекция объектов [deviceCategory](../resources/intune-shared-devicecategory.md)|Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Получение объекта deviceCategory](../api/intune-shared-devicecategory-get.md)|[deviceCategory](../resources/intune-shared-devicecategory.md);|Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Создание объекта deviceCategory](../api/intune-shared-devicecategory-create.md)|[deviceCategory](../resources/intune-shared-devicecategory.md)|Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Удаление объекта deviceCategory](../api/intune-shared-devicecategory-delete.md)|Нет|Удаление объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Обновление объекта deviceCategory](../api/intune-shared-devicecategory-update.md)|[deviceCategory](../resources/intune-shared-devicecategory.md);|Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории устройства. Только для чтения.|
|**Входящая миграция**|
|displayName|Строка|Отображаемое имя категории устройств.|
|description|String|Необязательное описание категории устройств.|

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



