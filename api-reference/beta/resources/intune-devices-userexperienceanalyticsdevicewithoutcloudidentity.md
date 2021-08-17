---
title: тип ресурса userExperienceAnalyticsDeviceWithoutCloudIdentity
description: Устройство аналитики пользовательского интерфейса без облачной идентификации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0a6560696ccce4360c33fce65bb83b8a78d25f92b022677761cf2a51fa0fde56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54126922"
---
# <a name="userexperienceanalyticsdevicewithoutcloudidentity-resource-type"></a>тип ресурса userExperienceAnalyticsDeviceWithoutCloudIdentity

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Устройство аналитики пользовательского интерфейса без облачной идентификации.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userExperienceAnalyticsDeviceWithoutCloudIdentities](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-list.md)|[коллекция userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|Список свойств и связей [объектов userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|
|[Get userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-get.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|Чтение свойств и связей [объекта userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|
|[Создание userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-create.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|Создание нового [объекта userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|
|[Удаление userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-delete.md)|Нет|Удаляет объект [userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|
|[Обновление userExperienceAnalyticsDeviceWithoutCloudIdentity](../api/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity-update.md)|[userExperienceAnalyticsDeviceWithoutCloudIdentity](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|Обновление свойств объекта [userExperienceAnalyticsDeviceWithoutCloudIdentity.](../resources/intune-devices-userexperienceanalyticsdevicewithoutcloudidentity.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор устройства для клиентской аналитики пользовательского интерфейса.|
|deviceName|String|Клиент прикрепит имя устройства.|
|azureAdDeviceId|Строка|Azure Active Directory Id устройства|

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




