---
title: Тип ресурса Девицеманажементабстракткомплекссеттингинстанце
description: Экземпляр параметра, представляющий сложное значение для абстрактного параметра
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9b5f7e01002c08a206ffe776e3145f67ba0bc921
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34979427"
---
# <a name="devicemanagementabstractcomplexsettinginstance-resource-type"></a>Тип ресурса Девицеманажементабстракткомплекссеттингинстанце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий сложное значение для абстрактного параметра


Наследуется от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементабстракткомплекссеттингинстанцес](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-list.md)|Коллекция [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|Список свойств и связей объектов [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .|
|[Получение Девицеманажементабстракткомплекссеттингинстанце](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-get.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|Чтение свойств и связей объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .|
|[Создание Девицеманажементабстракткомплекссеттингинстанце](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-create.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|Создание нового объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .|
|[Удаление Девицеманажементабстракткомплекссеттингинстанце](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-delete.md)|Нет|Удаляет объект [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).|
|[Обновление Девицеманажементабстракткомплекссеттингинстанце](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-update.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|Обновление свойств объекта [девицеманажементабстракткомплекссеттингинстанце](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|Дефинитионид|String|Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|Валуежсон|String|Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|Имплементатионид|String|Идентификатор определения для выбранной реализации этого сложного параметра|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|значение|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Значения, составляющие сложный параметр|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAbstractComplexSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "implementationId": "String"
}
```





