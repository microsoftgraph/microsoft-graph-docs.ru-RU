---
title: тип ресурса remoteAssistanceReporting
description: Ресурсы RemoteAssistanceReporting представляют метаданные данной полезной нагрузки отчетов о удаленной помощи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2fb437a3b6b2cb44f32cc1e12a601b3ed4673ac
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61338143"
---
# <a name="remoteassistancereporting-resource-type"></a>тип ресурса remoteAssistanceReporting

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурсы RemoteAssistanceReporting представляют метаданные данной полезной нагрузки отчетов о удаленной помощи

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для сеанса и для полезной нагрузки отчетов каждого сеанса|
|startDateTime|DateTimeOffset|Время начала сеанса|
|endDateTime|DateTimeOffset|Время окончания сеанса|
|remoteAssistanceSessionType|[remoteAssistanceSessionType](../resources/intune-remoteassistance-remoteassistancesessiontype.md)|Тип сеанса удаленной помощи, который был проведен. Возможные значения: `viewOnly`, `fullControl`, `elevation`. Возможные значения: `viewOnly`, `fullControl`, `elevation`.|
|helperEmail|Строка|Электронная почта входа, используемая помощником для создания сеанса|
|helperTenantId|String|ID клиента для помощника|
|helperFirstName|Строка|Имя помощника|
|helperLastName|Строка|Фамилия помощника|
|helperOs|Строка|Операционная система помощника|
|helperDeviceAadId|String|ID устройства помощника AAD|
|helperDeviceName|Строка|Имя устройства помощника|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние регистрации intune устройства помощника. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|String|Электронная почта входа, используемая sharer для создания сеанса|
|sharerTenantId|Строка|ID клиента для sharer|
|sharerFirstName|Строка|Имя sharer|
|sharerLastName|Строка|Фамилия sharer|
|sharerDeviceAadId|String|ID устройства sharer AAD|
|sharerDeviceName|Строка|Имя устройства sharer|
|sharerOs|String|Операционная система Sharer|
|sharerEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние регистрации intune устройства sharer. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|

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




