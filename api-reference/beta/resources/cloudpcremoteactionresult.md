---
title: тип ресурса cloudPcRemoteActionResult
description: Представляет удаленный результат действия, заданный облачным КОМПЬЮТЕРом.
author: RuiHou105
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 9b708df825104cd85175543b7c16850c16d40d0d
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336027"
---
# <a name="cloudpcremoteactionresult-resource-type"></a>тип ресурса cloudPcRemoteActionResult

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет удаленный результат действия, заданный облачным КОМПЬЮТЕРом.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[getCloudPcRemoteActionResults](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Проверьте удаленные результаты действий, указанные на облачном компьютере. Облачный компьютер поддерживает повторное и повторное управление удаленными действиями.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|actionName|String|Указанное действие. Поддерживаемые значения на Microsoft Endpoint Manager: `Reprovision`, . `Resize``Restore` Поддерживаемые значения в корпоративных устройствах облачных ПК: `Reboot`, , `Rename``Reprovision`, `Troubleshoot`.|
|actionState|[actionState](#actionstate-values)|Состояние действия. Возможные значения: `None`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`. Только для чтения.|
|cloudPcId|Строка|ID устройства облачного ПК, на котором выполняется удаленное действие. Только для чтения.|
|managedDeviceId|Строка|ID управляемого устройства Intune, на котором выполняется удаленное действие. Только для чтения.|
|startDateTime|DateTimeOffset|Время начала действия. Timestamp показан в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, полночь UTC 1 января 2014 г. отображается как '2014-01-01T00:00:00Z'.|
|lastUpdatedDateTime|DateTimeOffset|Время последнего обновления для действий. Timestamp показан в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, полночь UTC 1 января 2014 г. отображается как '2014-01-01T00:00:00Z'.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcStatusDetails.md)|Сведения о состоянии облачного КОМПЬЮТЕРА. |

### <a name="actionstate-values"></a>значения actionState

|Member|Описание|
|:---|:---|
|Нет|Не является допустимым состоянием действия.|
|ожидание|Действие ожидается.|
|отменено|Действие отменено.|
|active|Действие активно.|
|done|Действие выполнено без ошибок.|
|не удалось|Действие не удалось.|
|notSupported|Действие не поддерживается.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.cloudPcRemoteActionResult"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcRemoteActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)",
  "cloudPcId": "String",
  "managedDeviceId": "String",
  "statusDetails": {
    "@odata.type": "microsoft.graph.cloudPcStatusDetails"
  }
}
```
