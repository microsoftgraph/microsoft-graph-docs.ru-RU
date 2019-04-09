---
title: Тип ресурса Девицеманажементсеттингинстанце
description: Базовый тип для экземпляра параметра
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9aef844dd4957b75b51f8d16014c2253b0253cc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523611"
---
# <a name="devicemanagementsettinginstance-resource-type"></a>Тип ресурса Девицеманажементсеттингинстанце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Базовый тип для экземпляра параметра

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементсеттингинстанцес](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Список свойств и связей объектов [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .|
|[Получение Девицеманажементсеттингинстанце](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[Девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Чтение свойств и связей объекта [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор экземпляра параметра|
|Дефинитионид|String|Идентификатор определения параметра для этого экземпляра.|
|Валуежсон|String|Представление значения в формате JSON|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```







