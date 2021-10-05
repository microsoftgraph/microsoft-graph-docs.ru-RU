---
title: тип ресурса deviceRegistrationPolicy
description: Представляет область политики, контролируемую ограничениями квот, дополнительной проверкой подлинности и политиками авторизации для Azure Active Directory клиента.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 6733937ce5edf2f224b652b1659fe951f101b914
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127946"
---
# <a name="deviceregistrationpolicy-resource-type"></a>тип ресурса deviceRegistrationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет область политики, контролируемую ограничениями квот, дополнительной проверкой подлинности и политиками авторизации для регистрации удостоверений устройств в организации.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Get deviceRegistrationPolicy](../api/deviceregistrationpolicy-get.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|Ознакомьтесь с свойствами [объекта deviceRegistrationPolicy.](../resources/deviceregistrationpolicy.md)|
|[Обновление deviceRegistrationPolicy](../api/deviceregistrationpolicy-update.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|Обновление свойств объекта [deviceRegistrationPolicy.](../resources/deviceregistrationpolicy.md)|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|Указывает политику авторизации для контроля регистрации новых устройств с помощью **Azure AD Join** в организации. Обязательный. Дополнительные сведения см. [в том, что такое удостоверение устройства?](/azure/active-directory/devices/overview).|
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|Указывает политику авторизации для контроля регистрации новых устройств с помощью **Azure AD, зарегистрированных** в организации. Обязательно. Дополнительные сведения см. [в том, что такое удостоверение устройства?](/azure/active-directory/devices/overview).|
|description|Строка|Описание политики регистрации устройств. Он всегда настроен на `Device Registration Policy` . Только для чтения.|
|displayName|Строка|Имя политики регистрации устройств. Он всегда настроен на `Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks` . Только для чтения.|
|id|String| Идентификатор политики регистрации устройств. Он всегда настроен на `deviceRegistrationPolicy` . Только для чтения.|
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|Указывает политику проверки подлинности, чтобы пользователь завершил регистрацию с помощью **Azure AD Join** или **Azure AD, зарегистрированных** в организации. Возможные значения: `notRequired` , `required` , `unknownFutureValue` . Значение по умолчанию — `notRequired`. |
|userDeviceQuota|Int32|Указывает максимальное количество устройств, которые пользователь может иметь в организации, перед блокировкой регистрации новых устройств. Значение по умолчанию установлено до 50. Если это свойство не указано во время операции обновления политики, оно автоматически сбрасывается, чтобы указать, что пользователям не разрешено присоединяться `0` к любым устройствам. |


## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление в формате JSON

Ниже указано представление ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceRegistrationPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceRegistrationPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userDeviceQuota": "Integer",
  "multiFactorAuthConfiguration": "String",
  "azureADRegistration": {
    "@odata.type": "microsoft.graph.azureADRegistrationPolicy"
  },
  "azureADJoin": {
    "@odata.type": "microsoft.graph.azureAdJoinPolicy"
  }
}
```
