---
title: Тип ресурса remoteAssistanceReporting
description: Ресурсы RemoteAssistanceReporting представляют метаданные заданных полезных данных отчетов удаленного помощника
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 65ca73ed17e70e9d4a86439a1daea490b84b30bc
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668652"
---
# <a name="remoteassistancereporting-resource-type"></a>Тип ресурса remoteAssistanceReporting

Пространство имен: microsoft.graph

> **Важно:** API Microsoft Graph в версии /beta могут быть изменены; использование в рабочей области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурсы RemoteAssistanceReporting представляют метаданные заданных полезных данных отчетов удаленного помощника

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор сеанса и полезных данных отчетов каждого сеанса.|
|startDateTime|DateTimeOffset|Время начала сеанса|
|endDateTime|DateTimeOffset|Время окончания сеанса|
|remoteAssistanceSessionType|[remoteAssistanceSessionType](../resources/intune-remoteassistance-remoteassistancesessiontype.md)|Тип сеанса удаленной помощи, который был выполнен. Возможные значения: `viewOnly`, `fullControl`, `elevation`. Возможные значения: `viewOnly`, `fullControl`, `elevation`.|
|helperEmail|String|Адрес электронной почты для входа, используемый вспомогательной службой для установки сеанса|
|helperTenantId|String|Идентификатор клиента для вспомогательной службы|
|helperFirstName|String|Имя вспомогательной функции|
|helperLastName|String|Фамилия вспомогательной функции|
|вспомогательные объекты|String|Операционная система вспомогательной службы|
|helperDeviceAadId|String|Идентификатор AAD вспомогательного устройства|
|helperDeviceName|String|Имя устройства вспомогательной службы|
|helperEnrollmentState|[enrollmentState](../resources/intune-remoteassistance-enrollmentstate.md)|Intune состояние регистрации вспомогательного устройства. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|String|Адрес электронной почты для входа, используемый обработчиком для установки сеанса|
|sharerTenantId|String|Идентификатор клиента для общего ресурса|
|sharerFirstName|String|Имя sharer|
|sharerLastName|String|Фамилия sharer|
|sharerDeviceAadId|String|Идентификатор AAD устройства Sharer|
|sharerDeviceName|String|Имя устройства sharer|
|sharerOs|String|Операционная система Sharer|
|sharerEnrollmentState|[enrollmentState](../resources/intune-remoteassistance-enrollmentstate.md)|Intune состояние регистрации устройства общего ресурса. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.remoteAssistanceReporting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistanceReporting",
  "id": "String (identifier)",
  "startDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)",
  "remoteAssistanceSessionType": "String",
  "helperEmail": "String",
  "helperTenantId": "String",
  "helperFirstName": "String",
  "helperLastName": "String",
  "helperOs": "String",
  "helperDeviceAadId": "String",
  "helperDeviceName": "String",
  "helperEnrollmentState": "String",
  "sharerEmail": "String",
  "sharerTenantId": "String",
  "sharerFirstName": "String",
  "sharerLastName": "String",
  "sharerDeviceAadId": "String",
  "sharerDeviceName": "String",
  "sharerOs": "String",
  "sharerEnrollmentState": "String"
}
```




