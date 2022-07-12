---
title: Тип ресурса deviceCategory
description: Категории устройств используются для упорядочивания устройств. Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации. Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: cdf0d172efdc7dd91bc64301e42b0764c0cd882f
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/12/2022
ms.locfileid: "66730597"
---
# <a name="devicecategory-resource-type"></a>Тип ресурса deviceCategory

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Категории устройств используются для упорядочивания устройств. Используя категории устройств, администраторы могут определить собственные категории, применимые к их организации. Эти категории затем можно применить к устройству в консоли Azure Intune или выбрать во время регистрации устройства пользователем. На основе категорий устройств вы можете фильтровать отчеты и создавать динамические группы устройств Azure Active Directory.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Перечисление объектов deviceCategory](../api/intune-onboarding-devicecategory-list.md)|Коллекция объектов [deviceCategory](../resources/intune-onboarding-devicecategory.md)|Список свойств и связей объектов [deviceCategory](../resources/intune-onboarding-devicecategory.md).|
|[Получение объекта deviceCategory](../api/intune-onboarding-devicecategory-get.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|Чтение свойств и связей объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).|
|[Создание объекта deviceCategory](../api/intune-onboarding-devicecategory-create.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|Создание объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).|
|[Удаление объекта deviceCategory](../api/intune-onboarding-devicecategory-delete.md)|Нет|Удаление объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).|
|[Обновление объекта deviceCategory](../api/intune-onboarding-devicecategory-update.md)|[deviceCategory](../resources/intune-onboarding-devicecategory.md)|Обновление свойств объекта [deviceCategory](../resources/intune-onboarding-devicecategory.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор категории устройства. Только для чтения.|
|displayName|String|Отображаемое имя категории устройств.|
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





