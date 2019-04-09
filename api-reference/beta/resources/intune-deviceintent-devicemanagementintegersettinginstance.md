---
title: Тип ресурса Девицеманажементинтежерсеттингинстанце
description: Экземпляр параметра, представляющий значение целого числа
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 568a1d60572123424869f1ee98c3cb6bc600d36f
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522554"
---
# <a name="devicemanagementintegersettinginstance-resource-type"></a>Тип ресурса Девицеманажементинтежерсеттингинстанце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий значение целого числа


НаСледуется от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементинтежерсеттингинстанцес](../api/intune-deviceintent-devicemanagementintegersettinginstance-list.md)|Коллекция [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|Список свойств и связей объектов [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .|
|[Получение Девицеманажементинтежерсеттингинстанце](../api/intune-deviceintent-devicemanagementintegersettinginstance-get.md)|[Девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|Чтение свойств и связей объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .|
|[Создание Девицеманажементинтежерсеттингинстанце](../api/intune-deviceintent-devicemanagementintegersettinginstance-create.md)|[Девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|Создание нового объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .|
|[Удаление Девицеманажементинтежерсеттингинстанце](../api/intune-deviceintent-devicemanagementintegersettinginstance-delete.md)|Нет|Удаляет объект [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).|
|[Обновление Девицеманажементинтежерсеттингинстанце](../api/intune-deviceintent-devicemanagementintegersettinginstance-update.md)|[Девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)|Обновление свойств объекта [девицеманажементинтежерсеттингинстанце](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|Дефинитионид|String|Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|Валуежсон|String|Представление JSON значения, наСледуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|Int32|Целое значение|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntegerSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": 1024
}
```







