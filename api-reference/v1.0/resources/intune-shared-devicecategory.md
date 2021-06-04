---
title: Тип ресурса deviceCategory
description: Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 067e7894cc5c5daa4cd73c5bb5ba88f66b283366
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732758"
---
# <a name="devicecategory-resource-type"></a>Тип ресурса deviceCategory

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Категории устройств используются для упорядочивания устройств. Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации. Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Коллекция list deviceCategories](../api/intune-shared-devicecategory-list.md)|Список свойств и связей объектов [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Получение объекта deviceCategory](../api/intune-shared-devicecategory-get.md)|Чтение свойств и связей объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Создание объекта deviceCategory](../api/intune-shared-devicecategory-create.md)|Создание объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|
|[Удаление deviceCategory](../api/intune-shared-devicecategory-delete.md).|
|[Обновление объекта deviceCategory](../api/intune-shared-devicecategory-update.md)|Обновление свойств объекта [deviceCategory](../resources/intune-shared-devicecategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории устройства. Только для чтения.|
|**Адаптация**|
|displayName|String|Отображаемое имя категории устройств.|
|description|String|Необязательное описание категории устройств.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```









