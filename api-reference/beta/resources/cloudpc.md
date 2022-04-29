---
title: Тип ресурса cloudPC
description: Виртуальные рабочие столы, управляемые облаком.
author: AshleyYangSZ
ms.localizationpriority: medium
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: a4f43588966d060e79663ce20b945b9fee47ebb2
ms.sourcegitcommit: 4ef29d4a2cfa1ccc4a3da649e683377b17b90108
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/29/2022
ms.locfileid: "65125900"
---
# <a name="cloudpc-resource-type"></a>Тип ресурса cloudPC

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет управляемый облаком виртуальный рабочий стол. Этот облачный компьютер также регистрируется в Intune и управляется с помощью портала Microsoft Endpoint Manager, поэтому облачный компьютер также имеет соответствующий идентификатор Intune управляемого устройства.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Перечисление облачных компьютеров](../api/virtualendpoint-list-cloudpcs.md)|[Коллекция cloudPC](../resources/cloudpc.md)|Список свойств и связей объектов [cloudPC](../resources/cloudpc.md) .|
|[Получение cloudPC](../api/cloudpc-get.md)|[CloudPC](../resources/cloudpc.md)|Чтение свойств и связей объекта [cloudPC](../resources/cloudpc.md) .|
|[Изменение типа учетной записи пользователя](../api/cloudpc-changeuseraccounttype.md)|Нет|Изменение типа учетной записи пользователя на определенном облачном компьютере.|
|[Окончание льготного периода](../api/cloudpc-endgraceperiod.md)|Нет|Завершение льготного периода для [объекта cloudPC](../resources/cloudpc.md) .|
|[Получение результатов удаленного действия](../api/manageddevice-getcloudpcremoteactionresults.md)|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Проверьте результаты удаленного действия, заданного [облачным компьютером](../resources/cloudpcremoteactionresult.md) , для устройства с облачным компьютером.|
|[Перезагрузки](../api/cloudpc-reboot.md)|Нет|Перезагрузите определенный [объект cloudPC](../resources/cloudpc.md) .|
|[Rename](../api/cloudpc-rename.md)|Нет|Переименуйте [определенный объект cloudPC](../resources/cloudpc.md) . Используйте этот API для обновления **displayName** для сущности Облачного компьютера.|
|[Повторная подготовка](../api/cloudpc-reprovision.md)|Нет|Повторно подготовить объект [cloudPC](../resources/cloudpc.md) .|
|[Удаленное действие повторной подготовки](../api/manageddevice-reprovisioncloudpc.md)|Нет|Повторно подготовьте облачный компьютер с Intune [неуправляемого](../resources/cloudpc.md) устройства.  |
|[Удаленное действие массовой повторной подготовки](../api/manageddevice-bulkreprovisioncloudpc.md)|Нет|Массовая повторная подготовка набора облачных компьютеров с Intune управляемых устройств.|
|[Изменение размера удаленного действия](../api/manageddevice-resizecloudpc.md)|Нет|Обновите или понизите уровень существующего облачного компьютера до другой конфигурации с новым виртуальным ЦП и размером хранилища с Intune управляемого устройства.|
|[Устранение неполадок](../api/cloudpc-troubleshoot.md)|Нет|Устранение неполадок [определенного объекта cloudPC](../resources/cloudpc.md) . Используйте этот API для проверки состояния работоспособности облачного компьютера и узла сеанса.|
|[Восстановление удаленного действия](../api/manageddevice-restorecloudpc.md)|Нет|Восстановление устройства облачного компьютера до предыдущего состояния из моментального снимка.|
|[Удаленное действие массового восстановления](../api/manageddevice-bulkrestorecloudpc.md)|[cloudPcBulkRemoteActionResult](../resources/cloudpcbulkremoteactionresult.md)|Восстановите несколько облачных устройств с одним запросом, который включает идентификаторы Intune управляемых устройств, а также дату и время точки восстановления.|
|[Список для пользователя](../api/user-list-cloudpcs.md)|[Коллекция cloudPC](../resources/cloudpc.md)|Список устройств [CloudPC](../resources/cloudpc.md) , которые назначены вошедаму пользователю.|
|[Получение сведений о запуске для пользователя](../api/cloudpc-getcloudpclaunchinfo.md)|[cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md)|Получите [cloudPCLaunchInfo](../resources/cloudpclaunchinfo.md) для пользователя, выполнившего вход.|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|aadDeviceId|String|Идентификатор Azure Active Directory (Azure AD) облачного компьютера.|
|displayName|String|Отображаемое имя облачного компьютера.|
|gracePeriodEndDateTime|DateTimeOffset|Дата и время окончания льготного периода и повторной подготовки или отзыва. Требуется только в том случае, если состояние равно .`inGracePeriod` Метка времени отображается в формате ISO 8601 и времени в формате UTC. Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|id|String|Уникальный идентификатор облачного компьютера. Только для чтения.|
|imageDisplayName|String|Имя образа ОС, который содержится на облачном компьютере.|
|lastLoginResult|[cloudPcLoginResult](../resources/cloudpcloginresult.md)|Результат последнего входа облачного компьютера. Например, `{ "time": "2014-01-01T00:00:00Z"}`.|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения облачного компьютера. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|
|lastRemoteActionResult|[cloudPcRemoteActionResult](../resources/cloudpcremoteactionresult.md)|Результат последнего удаленного действия корпоративных облачных компьютеров. Поддерживаются следующие удаленные действия: , , , и `Troubleshoot``Restore`. `Reprovision``Rename``Reboot`|
|managedDeviceId|String|Идентификатор Intune устройства облачного компьютера.|
|managedDeviceName|String|Имя Intune устройства облачного компьютера.|
|onPremisesConnectionName|String|Сетевое подключение Azure, которое применяется во время подготовки облачных компьютеров.|
|osVersion|[cloudPcOperatingSystem](../resources/cloudpcorganizationsettings.md#cloudpcoperatingsystem-values)|Версия операционной системы (ОС) для подготовки на облачных компьютерах. Возможные значения: `windows10`, и `windows11``unknownFutureValue`.|
|provisioningPolicyId|String|Идентификатор политики подготовки облачного компьютера.|
|provisioningPolicyName|String|Политика подготовки, применяемая во время подготовки облачных компьютеров.|
|servicePlanId|String|Идентификатор плана обслуживания облачного компьютера.|
|servicePlanName|String|Имя плана обслуживания облачного компьютера.|
|servicePlanType|[cloudPcServicePlanType](../resources/cloudpcserviceplan.md#cloudpcserviceplantype-values)|Тип плана обслуживания облачного компьютера.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Состояние облачного компьютера. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`, `restoring`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Сведения о состоянии облачного компьютера.|
|userAccountType|[CloudPcUserAccountType](../resources/cloudpcorganizationsettings.md#cloudpcuseraccounttype-values)|Тип учетной записи пользователя на подготовленных облачных компьютерах. Возможные значения: `standardUser`, и `administrator``unknownFutureValue`.|
|userPrincipalName|String|Имя участника-пользователя (UPN) пользователя, назначенного облачному компьютеру.|

### <a name="cloudpcstatus-values"></a>Значения cloudPcStatus

|Member|Описание|
|:---|:---|
|notProvisioned|Облачный компьютер не был подготовлен.|
|Подготовки|Выполняется подготовка облачных компьютеров.|
|Подготовлено|Облачный компьютер подготовлен и может быть доступен конечным пользователям.|
|inGracePeriod|Облачный компьютер находится в льготном периоде за одну неделю до отзыва.|
|отмена подготовки|Облачный компьютер отозван.|
|Сбой при|Сбой операции на облачном компьютере.|
|provisionedWithWarnings|Облачный компьютер подготовлен и может быть доступен конечным пользователям, но с некоторыми предупреждениями. Пользователь может продолжать использовать этот облачный компьютер.|
|Изменение размера|Размер облачного компьютера будет меняться.|
|pendingProvision|Подготовка ожидается на облачном компьютере. В этом случае количество облачных компьютеров в льготный период превышает общее количество доступных лицензий. |
|Восстановление|Облачный компьютер восстанавливается.|
|unknownFutureValue|Значение sentinel для развиваемого перечисления. Не следует использовать.|

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
