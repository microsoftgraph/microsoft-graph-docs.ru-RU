---
title: Тип ресурса userExperienceAnalyticsDeviceWithoutCloudIdentity
description: Устройство аналитики пользовательского интерфейса без облачного удостоверения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3a747d145498aaea3d349ab9ac5e2b3efe51b583
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160972"
---
# <a name="userexperienceanalyticsdevicewithoutcloudidentity-resource-type"></a>Тип ресурса userExperienceAnalyticsDeviceWithoutCloudIdentity

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в бета-версии могут изменяться; использование в производственной области не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройство аналитики пользовательского интерфейса без облачного удостоверения.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsDeviceWithoutCloudIdentities](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-list.md)|[Коллекция userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|Список свойств и связей [объектов userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|
|[Get userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-get.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|Чтение свойств и связей объекта [userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|
|[Создание объекта userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-create.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|Создание объекта [userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|
|[Удаление userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-delete.md)|Нет|Удаляет [userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|
|[Обновление объекта userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-update.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства с присоединением клиента аналитики пользовательского интерфейса.|
|deviceName|String|Имя устройства с присоединением клиента.|
|azureAdDeviceId|String|ИД устройства Azure Active Directory|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceWithoutCloudIdentity",
  "id": "String (identifier)",
  "deviceName": "String",
  "azureAdDeviceId": "String"
}
```




