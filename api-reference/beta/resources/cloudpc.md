---
title: Тип ресурса cloudPC
description: Облачные управляемые виртуальные настольные компьютеры.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: 232ad6a8de6634f028ec59080114110c902ce184
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787501"
---
# <a name="cloudpc-resource-type"></a>Тип ресурса cloudPC

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет виртуальный рабочий стол с облачным управлением.

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[CloudPCs списка](../api/virtualendpoint-list-cloudpcs.md)|[коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)|
|[Get cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPC.](../resources/cloudpc.md)|
|[Reprovision](../api/cloudpc-reprovision.md)|Нет|Reprovision a [cloudPC](../resources/cloudpc.md) object.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для облачного КОМПЬЮТЕРА. Только для чтения.|
|displayName|String|Имя отображения облачного КОМПЬЮТЕРА.|
|imageDisplayName|String|Имя изображения ОС на облачном компьютере.|
|managedDeviceId|String|ID устройства Intune облачного компьютера.|
|managedDeviceName|String|Имя устройства Intune облачного КОМПЬЮТЕРА.|
|provisioningPolicyId|String|ID политики обеспечения облачного компьютера.|
|provisioningPolicyName|String|Политика обеспечения, применяемая при обеспечении облачных компьютеров.|
|onPremisesConnectionName|String|Локальное подключение, применяемого при обеспечении облачных компьютеров.|
|servicePlanId|String|ID плана службы облачного КОМПЬЮТЕРА.|
|servicePlanName|String|Имя плана службы облачного КОМПЬЮТЕРА.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Состояние облачного КОМПЬЮТЕРА. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Сведения о состоянии облачного КОМПЬЮТЕРА.|
|userPrincipalName|String|Основное имя пользователя (UPN) пользователя, назначенного на облачный КОМПЬЮТЕР.|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время облачного компьютера. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|gracePeriodEndDateTime|DateTimeOffset|Дата и время окончания льготного периода и переделки/депрограммивинга. Требуется только в том случае, если состояние `inGracePeriod` . Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

### <a name="cloudpcstatus-values"></a>значения cloudPcStatus

|Member|Описание|
|:---|:---|
|notProvisioned|Этот Cloud PC не был предварительно.|
|подготовка|Cloud PC подготовка продолжается.|
|provisioned|Подготовка Cloud PC и доступ к нему могут получить конечные пользователи.|
|обновление|Cloud PC продолжается.|
|inGracePeriod|Срок Cloud PC находится в периоде отсрочки за одну неделю до его деразвения.|
|deprovisioning|The Cloud PC deprovisioning.|
|не удалось|Операция на Cloud PC не удалась.|

## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPC",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPC",
  "id": "String (identifier)",
  "displayName": "String",
  "imageDisplayName": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)"
}
```
