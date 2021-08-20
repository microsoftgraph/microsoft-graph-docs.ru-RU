---
title: тип ресурса depEnrollmentBaseProfile
description: Ресурс DepEnrollmentBaseProfile представляет профиль программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bc1d9e84df78dbb990c859c0b770f3fe4998b524da0cf85bb7e4d123c69308b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54236075"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>тип ресурса depEnrollmentBaseProfile

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс DepEnrollmentBaseProfile представляет профиль программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.


Наследует [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[коллекция depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Список свойств и связей объектов [depEnrollmentBaseProfile.](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|[Получить depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Чтение свойств и связей объекта [depEnrollmentBaseProfile.](../resources/intune-enrollment-depenrollmentbaseprofile.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логический|Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Строка|URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал. Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логический|Указывает, Корпоративный портал требуется на устройствах, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли это профилем по умолчанию|
|supervisedModeEnabled|Логический|Режим Под контролем, True, чтобы включить, ложные в противном случае. Дополнительные https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune сведения см. в дополнительных сведениях.|
|supportDepartment|String|Сведения отдела поддержки|
|isMandatory|Логический|Указывает, является ли профиль обязательным|
|locationDisabled|Логический|Указывает, отключена ли панорама установки службы расположения|
|supportPhoneNumber|Строка|Номер телефона поддержки|
|profileRemovalDisabled|Логический|Указывает, отключен ли параметр удаления профиля|
|restoreBlocked|Логический|Указывает, заблокирована ли настройка области восстановления|
|appleIdDisabled|Логический|Указывает, отключена ли области установки apple id|
|termsAndConditionsDisabled|Логический|Указывает, отключено ли области установки "Условия и условия"|
|touchIdDisabled|Логический|Указывает, отключена ли настройка сенсорного id|
|applePayDisabled|Логический|Указывает, отключена ли система установки apple pay|
|siriDisabled|Логический|Указывает, отключено ли области настройки siri|
|diagnosticsDisabled|Логический|Указывает отключение области настройки диагностики|
|displayToneSetupDisabled|Логический|Указывает, отключен ли экран настройки displaytone|
|privacyPaneDisabled|Логический|Указывает, отключен ли экран конфиденциальности|
|screenTimeScreenDisabled|Логический|Указывает, отключена ли установка расстановки времени на экране|
|deviceNameTemplate|Строка|Задает буквальный или имя шаблон.|
|configurationWebUrl|Логический|URL-адрес входа помощника установки|

## <a name="relationships"></a>Связи
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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "String",
  "configurationWebUrl": true
}
```




