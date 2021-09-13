---
title: тип ресурса enrollmentProfile
description: Ресурс enrollmentProfile представляет коллекцию конфигураций, которые должны быть предоставлены для предварительной регистрации, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно постановлены. Для применения конфигураций профиля при регистрации соответствующего устройства этому типу профиля назначены предустановки устройств.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bae158fb33e4d1fccc4e5b4b6fd527b0d17cc9df
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59141090"
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
|[функция exportMobileConfig](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|Экспорт конфигурации мобильной связи|
|[Действие updateDeviceProfileAssignment](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|displayName|String|Имя профиля|
|description|String|Описание профиля|
|requiresUserAuthentication|Логический|Указывает, требует ли профиль проверки подлинности пользователя|
|configurationEndpointUrl|String|URL-адрес конечной точки конфигурации для регистрации|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал.|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логическое|Указывает, что Корпоративный портал требуется на устройствах, зарегистрированных помощником установки|

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



