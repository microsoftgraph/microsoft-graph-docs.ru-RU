---
title: Тип ресурса cloudPC
description: Облачные управляемые виртуальные настольные компьютеры.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e3f716b059a55f12add0eaf0b8ab785f71e1cb42
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59765202"
---
# <a name="cloudpc-resource-type"></a>Тип ресурса cloudPC

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет виртуальный рабочий стол с облачным управлением. Этот облачный компьютер также зарегистрирован в Intune и управляется через портал MEM, поэтому на облачном КОМПЬЮТЕРе также имеется соответствующий id управляемых устройств Intune.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[CloudPCs списка](../api/virtualendpoint-list-cloudpcs.md)|[коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)|
|[Get cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPC.](../resources/cloudpc.md)|
|[Reprovision](../api/cloudpc-reprovision.md)|Нет|Reprovision a [cloudPC](../resources/cloudpc.md) object.|
|[endGracePeriod](../api/cloudpc-endgraceperiod.md)|Нет|Окончание периода благодати для [объекта cloudPC.](../resources/cloudpc.md)|
|[Удаленное действие cloudPC reprovision](../api/manageddevice-reprovisioncloudpc.md)|Нет|Перенастройка облачного КОМПЬЮТЕРА с управляемым id устройствами Intune.|
|[Удаленное действие по массовому перепроизводство облачных компьютеров](../api/manageddevice-bulkreprovisioncloudpc.md)|Нет|Массовое перепроизводение набора устройств облачного ПК с управляемыми ID-устройствами Intune.|
|[Повторное удаленное действие cloudPC](../api/manageddevice-resizecloudpc.md)|Нет|Обновление или понижение существующего CloudPC в другую конфигурацию с новым vCPU и размером хранилища с помощью ID управляемого устройства Intune.|
|[Получить результаты удаленных действий cloudPC](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Проверьте удаленные результаты действий, [заданные](../resources/cloudpcremoteactionresult.md) облачным КОМПЬЮТЕРом, для устройства облачного ПК.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Уникальный идентификатор для облачного КОМПЬЮТЕРА. Только для чтения.|
|displayName|Строка|Имя отображения облачного КОМПЬЮТЕРА.|
|imageDisplayName|Строка|Имя изображения ОС, которое на облачном компьютере.|
|managedDeviceId|Строка|ID устройства Intune облачного компьютера.|
|managedDeviceName|String|Имя устройства Intune облачного КОМПЬЮТЕРА.|
|provisioningPolicyId|Строка|ID политики обеспечения облачного компьютера.|
|provisioningPolicyName|String|Политика продюсинга, применяемая при обеспечении облачных компьютеров.|
|onPremisesConnectionName|Строка|Локальное подключение, применяемого при обеспечении облачных компьютеров.|
|servicePlanId|Строка|ID плана службы облачного КОМПЬЮТЕРА.|
|servicePlanName|String|Имя плана службы облачного КОМПЬЮТЕРА.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Состояние облачного КОМПЬЮТЕРА. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Сведения о состоянии облачного КОМПЬЮТЕРА.|
|userPrincipalName|String|Основное имя пользователя (UPN) пользователя, назначенного на облачный компьютер.|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время облачного компьютера. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|gracePeriodEndDateTime|DateTimeOffset|Дата и время окончания льготного периода и переделки/депрограммивинга. Требуется только в том случае, если состояние `inGracePeriod` . Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

### <a name="cloudpcstatus-values"></a>значения cloudPcStatus

|Member|Описание|
|:---|:---|
|notProvisioned|Облачный КОМПЬЮТЕР не был предусмотрен.|
|подготовка|Подготовка облачного компьютера продолжается.|
|provisioned|Облачный компьютер является предварительным и может быть доступ к конечным пользователям.|
|inGracePeriod|Облачный компьютер находится в периоде отсрочки на одну неделю до его деразвения.|
|deprovisioning|Облачный КОМПЬЮТЕР развяжен.|
|не удалось|Операция на облачном компьютере не удалась.|
|provisionedWithWarnings|Облачный компьютер является предостережением и может быть доступ к конечным пользователям, но с некоторыми предупреждениями. Пользователь может продолжать использовать этот облачный КОМПЬЮТЕР.|
|resizing|Облачный КОМПЬЮТЕР имеет размер.|
|unknownFutureValue|Эволюционирующее значение sentinel. Не следует использовать.|

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
