---
title: тип ресурса remoteAssistanceReporting
description: Ресурсы RemoteAssistanceReporting представляют метаданные данной полезной нагрузки отчетов о удаленной помощи
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7793b8ef8bffa33e5d2e77de9fd102b9d0c59288
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039464"
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
|helperDeviceAadId|String|AAD-Id устройства помощника|
|helperDeviceName|String|Имя устройства помощника|
|helperEnrollmentState|[enrollmentState](../resources/intune-shared-enrollmentstate.md)|Состояние регистрации intune устройства помощника. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`. Возможные значения: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.|
|sharerEmail|String|Электронная почта входа, используемая sharer для создания сеанса|
|sharerTenantId|String|ID клиента для sharer|
|sharerFirstName|String|Имя sharer|
|sharerLastName|String|Фамилия sharer|
|sharerDeviceAadId|String|AAD-Id устройства Sharer|
|sharerDeviceName|String|Имя устройства sharer|
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



