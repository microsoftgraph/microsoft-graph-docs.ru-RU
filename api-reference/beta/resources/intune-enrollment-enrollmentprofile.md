---
title: Тип ресурса enrollmentProfile
description: Ресурс enrollmentProfile представляет коллекцию конфигураций, которым необходимо предоставить предварительной регистрации для включения регистрация некоторых устройствах, идентификаторы были предварительно разделены. Предварительно разделены устройства удостоверения назначаются этот тип профиля для применения настроек профиля в регистрации соответствующего устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a7ce4aac1e22610d539419dd6a63d124616b83f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396842"
---
# <a name="enrollmentprofile-resource-type"></a>Тип ресурса enrollmentProfile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс enrollmentProfile представляет коллекцию конфигураций, которым необходимо предоставить предварительной регистрации для включения регистрация некоторых устройствах, идентификаторы были предварительно разделены. Предварительно разделены устройства удостоверения назначаются этот тип профиля для применения настроек профиля в регистрации соответствующего устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) коллекции|Свойства списка и связей объектов [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Получение enrollmentProfile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Чтение свойства и связи объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Создание enrollmentProfile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Создание нового объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Удаление enrollmentProfile](../api/intune-enrollment-enrollmentprofile-delete.md)|Нет|Удаляет [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).|
|[Обновление enrollmentProfile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Обновление свойства объекта [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Действие setDefaultProfile](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|Нет|Н/Д|
|[функция exportMobileConfig](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|Экспорт конфигурации мобильных устройств|
|[Действие updateDeviceProfileAssignment](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|displayName|String|Имя профиля|
|description|String|Описание профиля|
|requiresUserAuthentication|Логический|Указывает необходимость проверки подлинности пользователей в профиле|
|configurationEndpointUrl|String|URL-адрес конечной точки конфигурации для подачи заявок|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки|

## <a name="relationships"></a>Отношения
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




