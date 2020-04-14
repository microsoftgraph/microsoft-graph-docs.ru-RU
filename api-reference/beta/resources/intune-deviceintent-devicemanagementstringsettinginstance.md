---
title: Тип ресурса Девицеманажементстрингсеттингинстанце
description: Экземпляр параметра, представляющий строковое значение
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0bdf26975143a922d71a3f63baa7032f6a469254
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419979"
---
# <a name="devicemanagementstringsettinginstance-resource-type"></a>Тип ресурса Девицеманажементстрингсеттингинстанце

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий строковое значение


Наследуется от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементстрингсеттингинстанцес](../api/intune-deviceintent-devicemanagementstringsettinginstance-list.md)|Коллекция [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Список свойств и связей объектов [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .|
|[Получение Девицеманажементстрингсеттингинстанце](../api/intune-deviceintent-devicemanagementstringsettinginstance-get.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Чтение свойств и связей объекта [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .|
|[Создание Девицеманажементстрингсеттингинстанце](../api/intune-deviceintent-devicemanagementstringsettinginstance-create.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Создание нового объекта [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .|
|[Удаление Девицеманажементстрингсеттингинстанце](../api/intune-deviceintent-devicemanagementstringsettinginstance-delete.md)|Нет|Удаляет объект [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).|
|[Обновление Девицеманажементстрингсеттингинстанце](../api/intune-deviceintent-devicemanagementstringsettinginstance-update.md)|[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)|Обновление свойств объекта [девицеманажементстрингсеттингинстанце](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|дефинитионид|String|Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|валуежсон|String|Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|String|Строковое значение|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementStringSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "value": "String"
}
```



