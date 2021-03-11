---
title: Тип ресурса cloudPC
description: Облачные управляемые виртуальные настольные компьютеры.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: resourcePageType
ms.openlocfilehash: c5fc858e29abf7d649b32991d9e30ce64cc0b632
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721616"
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
|servicePlanId|String|ID плана службы облачного КОМПЬЮТЕРА.|
|servicePlanName|String|Имя плана службы облачного КОМПЬЮТЕРА.|
|status|[cloudPcStatus](#cloudpcstatus-values)|Состояние облачного КОМПЬЮТЕРА. Возможные значения: `notProvisioned`, `provisioning`, `provisioned`, `upgrading`, `inGracePeriod`, `deprovisioning`, `failed`.|
|statusDetails|[cloudPcStatusDetails](../resources/cloudpcstatusdetails.md)|Сведения о состоянии облачного КОМПЬЮТЕРА.|
|userPrincipalName|String|Основное имя пользователя (UPN) пользователя, назначенного на облачный КОМПЬЮТЕР.|
|lastModifiedDateTime|DateTimeOffset|Последняя измененная дата и время облачного компьютера. Тип Timestamp представляет сведения о времени и дате с использованием формата ISO 8601 (всегда применяется формат UTC). Например, значение полуночи 1 января 2014 г. в формате UTC: `2014-01-01T00:00:00Z`.|

### <a name="cloudpcstatus-values"></a>значения cloudPcStatus

|Member|Описание|
|:---|:---|
|notProvisioned|Облачный КОМПЬЮТЕР не был предусмотрен.|
|подготовка|Подготовка облачного компьютера продолжается.|
|provisioned|Облачный компьютер является предварительным и может быть доступ к конечным пользователям.|
|обновление|В настоящее время идет процесс повторного окантовки облачного компьютера.|
|inGracePeriod|Облачный компьютер находится в периоде отсрочки на одну неделю до его деразвения.|
|deprovisioning|Облачный КОМПЬЮТЕР развяжен.|
|не удалось|Операция на облачном компьютере не удалась.|

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
  "servicePlanId": "String",
  "servicePlanName": "String",
  "status": "String",
  "userPrincipalName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```
