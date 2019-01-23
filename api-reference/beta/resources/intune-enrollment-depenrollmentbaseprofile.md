---
title: Тип ресурса depEnrollmentBaseProfile
description: Ресурс DepEnrollmentBaseProfile представляет профиля регистрации программы регистрации устройства Apple (DEP). Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b820959e5515a575e4f074a2762794a15e7f5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423757"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>Тип ресурса depEnrollmentBaseProfile

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс DepEnrollmentBaseProfile представляет профиля регистрации программы регистрации устройства Apple (DEP). Этот тип профиля должен быть назначен Apple DEP представленные числами, прежде чем соответствующих устройств можно зарегистрировать с помощью функции.


Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) коллекции|Свойства списка и связей объектов [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|
|[Получение depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Чтение свойства и связи объекта [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Идентификатор GUID для объекта унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|String|Имя профиля, унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логический|Указывает, если профиль требует проверки подлинности пользователя унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|String|Конфигурация конечную точку URL-адрес для регистрации наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании. Наследуется от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, что требуется портала компании на устройствах помощник по регистрации программы установки унаследованные от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Логический|Указывает, является ли профиля по умолчанию|
|supervisedModeEnabled|Логический|Режим контролируемом значение True для включения значение false в противном случае. Просмотреть https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune для получения дополнительных сведений.|
|supportDepartment|String|Сведения о поддержке отдела|
|passCodeDisabled|Логический|Указывает, если область настройки секретный код отключен|
|isMandatory|Логический|Указывает, является ли обязательных профилей|
|locationDisabled|Логический|Указывает, если область настройки расположения службы отключен|
|supportPhoneNumber|String|Номер телефона службы поддержки|
|profileRemovalDisabled|Логический|Указывает, если параметр удаления профиль отключен|
|restoreBlocked|Логический|Указывает, если область настройки восстановления блокируется|
|appleIdDisabled|Логический|Указывает, если область настройки идентификатор Apple отключен|
|termsAndConditionsDisabled|Логический|Указывает, если отключено «Сроками и условиями» область настройки|
|touchIdDisabled|Логический|Указывает, если область настройки идентификатор сенсорного ввода отключен|
|applePayDisabled|Логический|Указывает, если область настройки оплаты Apple отключен|
|zoomDisabled|Логический|Указывает, если область настройки масштаба отключен|
|siriDisabled|Логический|Указывает, если область настроек siri отключен|
|diagnosticsDisabled|Логический|Указывает, если область настройки диагностики отключен|
|displayToneSetupDisabled|Логический|Указывает, если экран установки displaytone отключен|
|privacyPaneDisabled|Логический|Указывает, если отключено экрана конфиденциальности|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true
}
```




