---
title: Тип ресурса Секуритибаселинекатегористатесуммари
description: Базовый план безопасности для каждой категории Сводка по состоянию соответствия требованиям для учетной записи базового уровня безопасности учетной записи.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f8fe826131e55df171e8c782d31ffc195c4a8a6f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419863"
---
# <a name="securitybaselinecategorystatesummary-resource-type"></a>Тип ресурса Секуритибаселинекатегористатесуммари

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый план безопасности для каждой категории Сводка по состоянию соответствия требованиям для учетной записи базового уровня безопасности учетной записи.


Наследуется от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Секуритибаселинекатегористатесуммариес](../api/intune-deviceintent-securitybaselinecategorystatesummary-list.md)|Коллекция [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Список свойств и связей объектов [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .|
|[Получение Секуритибаселинекатегористатесуммари](../api/intune-deviceintent-securitybaselinecategorystatesummary-get.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Чтение свойств и связей объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .|
|[Создание Секуритибаселинекатегористатесуммари](../api/intune-deviceintent-securitybaselinecategorystatesummary-create.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Создание нового объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .|
|[Удаление Секуритибаселинекатегористатесуммари](../api/intune-deviceintent-securitybaselinecategorystatesummary-delete.md)|Нет|Удаляет объект [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md).|
|[Обновление Секуритибаселинекатегористатесуммари](../api/intune-deviceintent-securitybaselinecategorystatesummary-update.md)|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)|Обновление свойств объекта [секуритибаселинекатегористатесуммари](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта. Наследуется от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|секурекаунт|Int32|Количество защищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|нотсекурекаунт|Int32|Количество незащищенных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|unknownCount|Int32|Количество неизвестных устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|errorCount|Int32|Количество устройств с ошибками, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|conflictCount|Int32|Количество устройств с конфликтами, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|notApplicableCount|Int32|Количество неприменимых устройств, наследуемых от [секуритибаселинестатесуммари](../resources/intune-deviceintent-securitybaselinestatesummary.md)|
|displayName|Строка|Имя категории|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineCategoryStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineCategoryStateSummary",
  "id": "String (identifier)",
  "secureCount": 1024,
  "notSecureCount": 1024,
  "unknownCount": 1024,
  "errorCount": 1024,
  "conflictCount": 1024,
  "notApplicableCount": 1024,
  "displayName": "String"
}
```



