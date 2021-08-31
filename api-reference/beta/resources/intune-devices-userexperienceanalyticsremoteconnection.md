---
title: тип ресурса userExperienceAnalyticsRemoteConnection
description: Пользовательский интерфейс аналитики объекта удаленного подключения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e9717b2865ff0e0a4126cc7f010925e8ff43360
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58820879"
---
# <a name="userexperienceanalyticsremoteconnection-resource-type"></a>тип ресурса userExperienceAnalyticsRemoteConnection

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Пользовательский интерфейс аналитики объекта удаленного подключения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsRemoteConnections](../api/intune-devices-userexperienceanalyticsremoteconnection-list.md)|[коллекция userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Список свойств и связей [объектов userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|
|[Get userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-get.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Чтение свойств и связей [объекта userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|
|[Создание userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-create.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Создание нового [объекта userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|
|[Удаление userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-delete.md)|Нет|Удаляет [пользователяExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md).|
|[Обновление userExperienceAnalyticsRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-update.md)|[userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Обновление свойств объекта [userExperienceAnalyticsRemoteConnection.](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|
|[summarizeDeviceRemoteConnection](../api/intune-devices-userexperienceanalyticsremoteconnection-summarizedeviceremoteconnection.md)|[коллекция userExperienceAnalyticsRemoteConnection](../resources/intune-devices-userexperienceanalyticsremoteconnection.md)|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор объекта удаленного подключения для аналитики пользовательского интерфейса.|
|deviceId|String|ID устройства.|
|deviceName|String|Имя устройства.|
|model|String|Модель устройства аналитики пользовательских интерфейсов.|
|virtualNetwork|String|Виртуальная сеть аналитики пользовательских интерфейсов.|
|manufacturer|String|Производитель аналитики пользовательских интерфейсов.|
|deviceCount|Int32|Количество удаленных подключений. Допустимые значения от 0 до 2147483647|
|cloudPcRoundTripTime|Двойное с плавающей точкой|Время круговой оконечности устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|cloudPcSignInTime|Двойное с плавающей точкой|Вход во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|remoteSignInTime|Двойное с плавающей точкой|Удаленный вход во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|coreBootTime|Двойное с плавающей точкой|Основное время загрузки устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|coreSignInTime|Двойное с плавающей точкой|Основной знак во время устройства облачного ПК. Допустимые значения от 0 до 1.79769313486232E+308|
|cloudPcFailurePercentage|Двойное с плавающей точкой|Вход в процент отказа облачного устройства PC. Допустимые значения: от 0 до 100|
|userPrincipalName|String|Пользователь с опытом аналитики userPrincipalName.|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsRemoteConnection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsRemoteConnection",
  "id": "String (identifier)",
  "deviceId": "String",
  "deviceName": "String",
  "model": "String",
  "virtualNetwork": "String",
  "manufacturer": "String",
  "deviceCount": 1024,
  "cloudPcRoundTripTime": "4.2",
  "cloudPcSignInTime": "4.2",
  "remoteSignInTime": "4.2",
  "coreBootTime": "4.2",
  "coreSignInTime": "4.2",
  "cloudPcFailurePercentage": "4.2",
  "userPrincipalName": "String"
}
```



