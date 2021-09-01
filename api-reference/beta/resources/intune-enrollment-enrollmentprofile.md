---
title: тип ресурса enrollmentProfile
description: Ресурс enrollmentProfile представляет коллекцию конфигураций, которые должны быть предоставлены для предварительной регистрации, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно постановлены. Для применения конфигураций профиля при регистрации соответствующего устройства этому типу профиля назначены предустановки устройств.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: eb5dc9a6d759e6f8a72097777b87d80a5dd33f5c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/31/2021
ms.locfileid: "58799791"
---
# <a name="enrollmentprofile-resource-type"></a>тип ресурса enrollmentProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс enrollmentProfile представляет коллекцию конфигураций, которые должны быть предоставлены для предварительной регистрации, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно постановлены. Для применения конфигураций профиля при регистрации соответствующего устройства этому типу профиля назначены предустановки устройств.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Регистрация спискаProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[коллекция enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|Список свойств и связей объектов [enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)|
|[Получить enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Чтение свойств и связей объекта [enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)|
|[Создание enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Создайте новый [объект enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)|
|[Удаление enrollmentProfile](../api/intune-enrollment-enrollmentprofile-delete.md)|Нет|Удаляет [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).|
|[Обновление enrollmentProfile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Обновление свойств объекта [enrollmentProfile.](../resources/intune-enrollment-enrollmentprofile.md)|
|[Действие setDefaultProfile](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|Нет|Н/Д|
|[функция exportMobileConfig](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|Строка|Экспорт конфигурации мобильной связи|
|[Действие updateDeviceProfileAssignment](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|displayName|Строка|Имя профиля|
|description|Строка|Описание профиля|
|requiresUserAuthentication|Boolean|Указывает, требует ли профиль проверки подлинности пользователя|
|configurationEndpointUrl|Строка|URL-адрес конечной точки конфигурации для регистрации|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал.|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, что Корпоративный портал требуется на устройствах, зарегистрированных помощником установки|

## <a name="relationships"></a>Связи
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```



