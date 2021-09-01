---
title: тип ресурса remoteAssistanceReporting
description: Ресурсы RemoteAssistanceReporting представляют метаданные данной полезной нагрузки отчетов о удаленной помощи
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d5442ce93f5e7697ed577835ddd437252396e67b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805358"
---
# <a name="remoteassistancereporting-resource-type"></a>тип ресурса remoteAssistanceReporting

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурсы RemoteAssistanceReporting представляют метаданные данной полезной нагрузки отчетов о удаленной помощи

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для сеанса и для полезной нагрузки отчетов каждого сеанса|
|startDateTime|DateTimeOffset|Время начала сеанса|
|endDateTime|DateTimeOffset|Время окончания сеанса|
|remoteAssistanceSessionType|[remoteAssistanceSessionType](../resources/intune-remoteassistance-remoteassistancesessiontype.md)|Тип сеанса удаленной помощи, который был проведен. Возможные значения: `viewOnly`, `fullControl`, `elevation`. Возможные значения: `viewOnly`, `fullControl`, `elevation`.|
|helperEmail|Строка|Электронная почта входа, используемая помощником для создания сеанса|
|helperTenantId|Строка|ID клиента для помощника|
|helperFirstName|Строка|Имя помощника|
|helperLastName|Строка|Фамилия помощника|
|helperDeviceAadId|Строка|AAD-Id устройства помощника|
|helperDeviceName|Строка|Имя устройства помощника|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние регистрации intune устройства помощника. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|Строка|Электронная почта входа, используемая sharer для создания сеанса|
|sharerTenantId|Строка|ID клиента для sharer|
|sharerFirstName|Строка|Имя sharer|
|sharerLastName|Строка|Фамилия sharer|
|sharerDeviceAadId|Строка|AAD-Id устройства Sharer|
|sharerDeviceName|Строка|Имя устройства sharer|
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
  "helperDeviceAadId": "String",
  "helperDeviceName": "String",
  "helperEnrollmentState": "String",
  "sharerEmail": "String",
  "sharerTenantId": "String",
  "sharerFirstName": "String",
  "sharerLastName": "String",
  "sharerDeviceAadId": "String",
  "sharerDeviceName": "String",
  "sharerEnrollmentState": "String"
}
```



