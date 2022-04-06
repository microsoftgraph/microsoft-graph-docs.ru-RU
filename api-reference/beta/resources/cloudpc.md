---
title: Тип ресурса cloudPC
description: Облачные управляемые виртуальные настольные компьютеры.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: cba73bf9f8d3281fe43400e90db9303bba69f36a
ms.sourcegitcommit: cc9e5b3630cb84c48bbbb2d84a963b9562d1fb78
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/31/2022
ms.locfileid: "64587667"
---
# <a name="cloudpc-resource-type"></a>Тип ресурса cloudPC

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет виртуальный рабочий стол с облачным управлением. Этот облачный КОМПЬЮТЕР также региструется в Intune и управляется через портал Microsoft Endpoint Manager, поэтому облачный ПК также имеет соответствующий Intune управляемый ID устройства.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[CloudPCs списка](../api/virtualendpoint-list-cloudpcs.md)|[коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC](../resources/cloudpc.md) .|
|[Get cloudPC](../api/cloudpc-get.md)|[cloudPC](../resources/cloudpc.md)|Ознакомьтесь с свойствами и отношениями объекта [cloudPC](../resources/cloudpc.md) .|
|[Изменение типа учетной записи пользователя](../api/cloudpc-changeuseraccounttype.md)|Нет|Измените тип учетной записи пользователя на определенном облачном компьютере.|
|[Окончание льготного периода](../api/cloudpc-endgraceperiod.md)|Нет|Окончание периода благодати для [объекта cloudPC](../resources/cloudpc.md) .|
|[Получить удаленные результаты действий](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Проверьте [удаленные результаты действий, заданные облачным КОМПЬЮТЕРом](../resources/cloudpcremoteactionresult.md) , для устройства облачного ПК.|
|[Перезагрузка](../api/cloudpc-reboot.md)|Нет|Перезагрузка определенного [объекта cloudPC](../resources/cloudpc.md) .|
|[Rename](../api/cloudpc-rename.md)|Нет|Переименование определенного [объекта cloudPC](../resources/cloudpc.md) . Используйте этот API для обновления **displayName** для объекта облачного ПК.|
|[Reprovision](../api/cloudpc-reprovision.md)|Нет|Reprovision a [cloudPC](../resources/cloudpc.md) object.|
|[Удаленное действие reprovision](../api/manageddevice-reprovisioncloudpc.md)|Нет|Перепроинделка облачного КОМПЬЮТЕРА с Intune [ID](../resources/cloudpc.md) устройства.  |
|[Массовое удаленное перепроизводство](../api/manageddevice-bulkreprovisioncloudpc.md)|Нет|Массовое перепроизводение набора устройств облачного ПК с Intune управляемыми ID-устройствами.|
|[Повторное удаленное действие](../api/manageddevice-resizecloudpc.md)|Нет|Обновление или понижение существующего облачного компьютера до другой конфигурации с новым vCPU и размером хранилища с Intune управляемым ID устройства.|
|[Устранение неполадок](../api/cloudpc-troubleshoot.md)|Нет|Устранение неполадок определенного [объекта cloudPC](../resources/cloudpc.md) . Используйте этот API для проверки состояния здоровья облачного компьютера и хоста сеанса.|
|[Восстановление удаленного действия](../api/manageddevice-restorecloudpc.md)|Нет|Восстановим устройство облачного ПК до предыдущего состояния из снимка.|
|[Массовое восстановление удаленного действия](../api/manageddevice-bulkrestorecloudpc.md)|[cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md)|Восстановление нескольких устройств облачного ПК с одним запросом, который включает Intune управляемых устройств и дату и время точки восстановления.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|aadDeviceId|Строка|ID Azure Active Directory (Azure AD) облачного компьютера.|
|displayName|Строка|Имя отображения облачного компьютера.|
|gracePeriodEndDateTime|DateTimeOffset|Дата и время окончания льготного периода и переделки/депрограммивинга. Требуется только в том случае, если состояние .`inGracePeriod` Timestamp отображается в формате ISO 8601 и Скоординированное универсальное время (UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|Строка|Уникальный идентификатор облачного компьютера. Только для чтения.|
|imageDisplayName|Строка|Имя изображения ОС, которое на облачном компьютере.|
|lastLoginResult|[cloudPcLoginResult](../resources/cloudpcloginresult.md)|Последний результат входа облачного компьютера. Например, `{ "time": "2014-01-01T00:00:00Z"}`.|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время облачного КОМПЬЮТЕРА. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastRemoteActionResult|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Последний результат удаленного действия корпоративных облачных компьютеров. Поддерживаемые удаленные действия: `Reboot`, , , `Reprovision`и `Troubleshoot``Restore``Rename`.|
|managedDeviceId|Строка|ID Intune устройства облачного компьютера.|
|managedDeviceName|String|Имя Intune устройства облачного КОМПЬЮТЕРА.|
|onPremisesConnectionName|String|Сетевое подключение Azure, применяемого во время подготовка облачных компьютеров.|
|osVersion|[cloudPcOperatingSystem](../resources/cloudpcorganizationsettings.md#cloudpcoperatingsystem-values)|Версия операционной системы (ОС) для обеспечения на облачных ПК. Возможные значения: `windows10`, и `windows11``unknownFutureValue`.|
|provisioningPolicyId|Строка|ID политики обеспечения облачного компьютера.|
|provisioningPolicyName|Строка|Политика обеспечения, применяемая при подготовках облачных компьютеров.|
|servicePlanId|String|ID плана службы облачного компьютера.|
|servicePlanName|String|Имя плана службы облачного компьютера.|
|servicePlanType|[cloudPcServicePlanType](../resources/cloudpcserviceplan.md#cloudpcserviceplantype-values)|Тип плана службы облачного компьютера.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Состояние облачного КОМПЬЮТЕРА. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`, `restoring`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Сведения о состоянии облачного КОМПЬЮТЕРА.|
|userAccountType|[cloudPcUserAccountType](../resources/cloudpcorganizationsettings.md#cloudpcuseraccounttype-values)|Тип учетной записи пользователя на предварительных облачных компьютерах. Возможные значения: `standardUser`, и `administrator``unknownFutureValue`.|
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
|pendingProvision|Подготовка ожидается на облачном компьютере. В этом случае количество облачных компьютеров в льготный период превышает общее количество доступных лицензий. |
|восстановление|Облачный компьютер восстанавливается.|
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
  "userAccountType": "String",
  "osVersion": "String",
  "lastRemoteActionResult": "String",
  "lastLoginResult": "String"
}
```
