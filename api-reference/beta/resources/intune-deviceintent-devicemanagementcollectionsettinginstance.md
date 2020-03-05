---
title: Тип ресурса Девицеманажементколлектионсеттингинстанце
description: Экземпляр параметра, представляющий коллекцию значений
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 06379bb1b3f43ce0fa1870632ccf575ccf415439
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528878"
---
# <a name="devicemanagementcollectionsettinginstance-resource-type"></a>Тип ресурса Девицеманажементколлектионсеттингинстанце

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий коллекцию значений


Наследуется от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементколлектионсеттингинстанцес](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-list.md)|Коллекция [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Список свойств и связей объектов [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .|
|[Получение Девицеманажементколлектионсеттингинстанце](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-get.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Чтение свойств и связей объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .|
|[Создание Девицеманажементколлектионсеттингинстанце](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-create.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Создание нового объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .|
|[Удаление Девицеманажементколлектионсеттингинстанце](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-delete.md)|Нет|Удаляет объект [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).|
|[Обновление Девицеманажементколлектионсеттингинстанце](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-update.md)|[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Обновление свойств объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|дефинитионид|String|Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|валуежсон|String|Представление JSON значения, наследуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|значение|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция значений|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```



