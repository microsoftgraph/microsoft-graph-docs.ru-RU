---
title: Тип ресурса Девицеманажементстрингсеттингинстанце
description: Экземпляр параметра, представляющий строковое значение
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3297085a905934792de2d371f295b467ad9a8e44
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562274"
---
# <a name="devicemanagementstringsettinginstance-resource-type"></a>Тип ресурса Девицеманажементстрингсеттингинстанце

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Экземпляр параметра, представляющий строковое значение


НаСледуется от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

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
|Дефинитионид|String|Идентификатор определения параметра для этого экземпляра, унаследованного от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|Валуежсон|String|Представление JSON значения, наСледуемого от [девицеманажементсеттингинстанце](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|value|String|Строковое значение|

## <a name="relationships"></a>Отношения
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





