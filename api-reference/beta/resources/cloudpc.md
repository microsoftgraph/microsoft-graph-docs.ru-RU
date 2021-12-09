---
title: Тип ресурса cloudPC
description: Облачные управляемые виртуальные настольные компьютеры.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: e2cc53304b7fea3336e8c52874e6c2bcf772b272
ms.sourcegitcommit: f336c5c49fbcebe55312656aa8b50511fd99a657
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/09/2021
ms.locfileid: "61391055"
---
# <a name="cloudpc-resource-type"></a>Тип ресурса cloudPC

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет виртуальный рабочий стол с облачным управлением. Этот облачный компьютер также зарегистрирован в Intune и управляется через портал Microsoft Endpoint Manager, поэтому облачный ПК также имеет соответствующий ID управляемого устройства Intune.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[CloudPCs списка](../api/virtualendpoint-list-cloudpcs.md)|[коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC.](../resources/cloudpc.md)|
|[Get cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPC.](../resources/cloudpc.md)|
|[Reprovision](../api/cloudpc-reprovision.md)|Нет|Reprovision a [cloudPC](../resources/cloudpc.md) object.|
|[Окончание льготного периода](../api/cloudpc-endgraceperiod.md)|Нет|Окончание периода благодати для [объекта cloudPC.](../resources/cloudpc.md)|
|[Перезагрузка](../api/cloudpc-reboot.md)|Нет|Перезагрузка определенного [объекта cloudPC.](../resources/cloudpc.md)|
|[Rename](../api/cloudpc-rename.md)|Нет|Переименование определенного [объекта cloudPC.](../resources/cloudpc.md) Используйте этот API для обновления **displayName** для объекта облачного ПК.|
|[Устранение неполадок](../api/cloudpc-troubleshoot.md)|Нет|Устранение неполадок определенного [объекта cloudPC.](../resources/cloudpc.md) Используйте этот API для проверки состояния здоровья облачного компьютера и хоста сеанса.|
|[Удаленное действие reprovision](../api/manageddevice-reprovisioncloudpc.md)|Нет|Перенастройка облачного компьютера [](../resources/cloudpc.md) с управляемым ИД устройства Intune.|
|[Массовое удаленное перепроизводство](../api/manageddevice-bulkreprovisioncloudpc.md)|Нет|Массовое перепроизводение набора устройств облачного ПК с управляемыми ID-устройствами Intune.|
|[Повторное удаленное действие](../api/manageddevice-resizecloudpc.md)|Нет|Обновление или понижение существующего облачного компьютера до другой конфигурации с новым vCPU и размером хранилища с помощью ID управляемого устройства Intune.|
|[Получить удаленные результаты действий](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Проверьте удаленные результаты действий, [заданные](../resources/cloudpcremoteactionresult.md) облачным КОМПЬЮТЕРом, для устройства облачного ПК.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|aadDeviceId|Строка|ID устройства Azure Active Directory Azure AD на облачном компьютере.|
|displayName|String|Имя отображения облачного компьютера.|
|gracePeriodEndDateTime|DateTimeOffset|Дата и время окончания льготного периода и переделки/депрограммивинга. Требуется только в том случае, если состояние `inGracePeriod` . Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|Строка|Уникальный идентификатор облачного компьютера. Только для чтения.|
|imageDisplayName|Строка|Имя изображения ОС, которое на облачном компьютере.|
|lastLoginResult|[cloudPcLoginResult](../resources/cloudpcloginresult.md)|Последний результат входа облачного компьютера. Например, `{ "time": "2014-01-01T00:00:00Z"}`.|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время облачного КОМПЬЮТЕРА. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastRemoteActionResult|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Последний результат удаленного действия корпоративных облачных компьютеров. Поддерживаемые удаленные действия: `Rename` `Reboot` , , и `Reprovision` `Troubleshoot` .|
|managedDeviceId|Строка|ID устройства Intune облачного компьютера.|
|managedDeviceName|String|Имя устройства Intune облачного КОМПЬЮТЕРА.|
|onPremisesConnectionName|Строка|Локальное подключение, применяемого при обеспечении облачных компьютеров.|
|provisioningPolicyId|Строка|ID политики обеспечения облачного компьютера.|
|provisioningPolicyName|Строка|Политика обеспечения, применяемая при подготовках облачных компьютеров.|
|servicePlanId|Строка|ID плана службы облачного компьютера.|
|servicePlanName|String|Имя плана службы облачного компьютера.|
|servicePlanType|[cloudPcServicePlanType](../resources/cloudpcserviceplan.md#cloudpcserviceplantype-values)|Тип плана службы облачного компьютера.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Состояние облачного КОМПЬЮТЕРА. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Сведения о состоянии облачного КОМПЬЮТЕРА.|
|userPrincipalName|String|Основное имя пользователя (UPN) пользователя, назначенного на облачный компьютер.|

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
  "aadDeviceId": "String",
  "managedDeviceId": "String",
  "managedDeviceName": "String",
  "provisioningPolicyId": "String",
  "provisioningPolicyName": "String",
  "onPremisesConnectionName": "String",
  "servicePlanId": "String",
  "servicePlanType": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "gracePeriodEndDateTime": "String (timestamp)",
  "lastRemoteActionResult": "String",
  "lastLoginResult": "String"
}
```
