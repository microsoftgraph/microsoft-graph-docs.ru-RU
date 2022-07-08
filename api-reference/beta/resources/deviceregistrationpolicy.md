---
title: Тип ресурса deviceRegistrationPolicy
description: Представляет область политики, которая управляет ограничениями квот, дополнительной проверкой подлинности и политиками авторизации для клиента Azure Active Directory.
author: myra-ramdenbourg
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: f810529cffc5c5c5c5a19d3fa2644aba5874d53e
ms.sourcegitcommit: c168f2cb95b4863080a84cc199a7b878fb5eeb8e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/08/2022
ms.locfileid: "66690083"
---
# <a name="deviceregistrationpolicy-resource-type"></a>Тип ресурса deviceRegistrationPolicy

Пространство имен: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Представляет область политики, которая управляет ограничениями квот, дополнительной проверкой подлинности и политиками авторизации для регистрации удостоверений устройств в организации.

## <a name="methods"></a>Методы

|Метод|Тип возвращаемых данных|Описание|
|:---|:---|:---|
|[Получение объекта deviceRegistrationPolicy](../api/deviceregistrationpolicy-get.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|Чтение свойств объекта [deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) .|
|[Обновление deviceRegistrationPolicy](../api/deviceregistrationpolicy-update.md)|[deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md)|Обновление свойств объекта [deviceRegistrationPolicy](../resources/deviceregistrationpolicy.md) .|

## <a name="properties"></a>Свойства

|Свойство|Тип|Описание|
|:---|:---|:---|
|azureADJoin|[azureAdJoinPolicy](../resources/azureadjoinpolicy.md)|Задает политику авторизации для управления регистрацией новых устройств с помощью **Azure AD** присоединения в организации. Обязательный элемент. Дополнительные сведения см. [в разделе "Что такое удостоверение устройства?"](/azure/active-directory/devices/overview).|
|azureADRegistration|[azureADRegistrationPolicy](../resources/azureadregistrationpolicy.md)|Задает политику авторизации для управления регистрацией новых устройств с помощью Azure AD **зарегистрированных** в организации. Обязательный элемент. Дополнительные сведения см. [в разделе "Что такое удостоверение устройства?"](/azure/active-directory/devices/overview).|
|description|Строка|Описание политики регистрации устройств. Для него всегда задано значение `Tenant-wide policy that manages intial provisioning controls using quota restrictions, additional authentication and authorization checks`. Только для чтения.|
|displayName|Строка|Имя политики регистрации устройств. Для него всегда задано значение `Device Registration Policy`. Только для чтения.|
|id|Строка| Идентификатор политики регистрации устройств. Для него всегда задано значение `deviceRegistrationPolicy`. Только для чтения.|
|multiFactorAuthConfiguration|multiFactorAuthConfiguration|Указывает политику проверки подлинности, с помощью Azure AD присоединения или Azure AD  регистрации **в организации**. Возможные значения: `0` (то есть `notRequired`), `1` (то есть `required`) и `2` (то есть `unknownFutureValue`). Значение по умолчанию — `0`. |
|userDeviceQuota|Int32|Указывает максимальное количество устройств, которые пользователь может иметь в вашей организации перед блокировкой регистрации новых устройств. Значение по умолчанию — 50. Если это свойство не указано во время операции обновления политики, `0` оно автоматически сбрасывается, чтобы указать, что пользователям не разрешено присоединяться к устройствам. |


## <a name="relationships"></a>Связи

Отсутствуют.

## <a name="json-representation"></a>Представление JSON

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
