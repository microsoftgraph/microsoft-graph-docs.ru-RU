---
title: тип ресурса remoteAssistanceReporting
description: Ресурсы RemoteAssistanceReporting представляют метаданные данной полезной нагрузки отчетов о удаленной помощи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 65103b951d41328d4e1b414a06ef99b8a99001bd
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/19/2021
ms.locfileid: "60485165"
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
|helperEmail|String|Электронная почта входа, используемая помощником для создания сеанса|
|helperTenantId|String|ID клиента для помощника|
|helperFirstName|String|Имя помощника|
|helperLastName|String|Фамилия помощника|
|helperOs|String|Операционная система помощника|
|helperDeviceAadId|String|ID устройства помощника AAD|
|helperDeviceName|String|Имя устройства помощника|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние регистрации intune устройства помощника. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|String|Электронная почта входа, используемая sharer для создания сеанса|
|sharerTenantId|String|ID клиента для sharer|
|sharerFirstName|String|Имя sharer|
|sharerLastName|String|Фамилия sharer|
|sharerDeviceAadId|String|ID устройства sharer AAD|
|sharerDeviceName|String|Имя устройства sharer|
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



