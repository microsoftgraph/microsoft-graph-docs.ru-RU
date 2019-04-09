---
title: Тип ресурса Девицеманажементколлектионсеттингинстанце
description: Экземпляр параметра, представляющий коллекцию значений
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31ce38adb753354c319a27e55cad8aa8a1e6024e
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524549"
---
# <a name="devicemanagementcollectionsettinginstance-resource-type"></a>Тип ресурса Девицеманажементколлектионсеттингинстанце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий коллекцию значений


НаСледуется от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Девицеманажементколлектионсеттингинстанцес](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-list.md)|Коллекция [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Список свойств и связей объектов [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .|
|[Получение Девицеманажементколлектионсеттингинстанце](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-get.md)|[Девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Чтение свойств и связей объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .|
|[Создание Девицеманажементколлектионсеттингинстанце](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-create.md)|[Девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Создание нового объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .|
|[Удаление Девицеманажементколлектионсеттингинстанце](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-delete.md)|Нет|Удаляет объект [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).|
|[Обновление Девицеманажементколлектионсеттингинстанце](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-update.md)|[Девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|Обновление свойств объекта [девицеманажементколлектионсеттингинстанце](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор экземпляра параметра, унаследованный от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|Дефинитионид|String|Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|Валуежсон|String|Представление JSON значения, наСледуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|

## <a name="relationships"></a>Связи
|Отношение|Тип|Описание|
|:---|:---|:---|
|value|Коллекция [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Коллекция значений|

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







