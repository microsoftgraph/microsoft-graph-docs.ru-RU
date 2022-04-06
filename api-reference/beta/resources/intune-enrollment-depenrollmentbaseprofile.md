---
title: тип ресурса depEnrollmentBaseProfile
description: Ресурс DepEnrollmentBaseProfile представляет профиль программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам DeP Apple, прежде чем соответствующие устройства смогут зарегистрироваться с помощью DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9b346e359922eb71fe55c9b84c6581ce2b7b0d8a
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630690"
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
|[Список depEnrollmentBaseProfiles](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|[коллекция depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Список свойств и связей объектов [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|
|[Получить depEnrollmentBaseProfile](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Чтение свойств и связей объекта [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID для объекта Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|Строка|Описание профиля, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requiresUserAuthentication|Логическое|Указывает, требует ли профиль проверки подлинности пользователя, унаследованной от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|configurationEndpointUrl|Строка|URL-адрес конечной точки конфигурации для использования для регистрации, унаследованной [от enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логическое|Указывает на проверку подлинности с помощью помощника установки Apple вместо Корпоративный портал. Унаследованный от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|requireCompanyPortalOnSetupAssistantEnrolledDevices|Логическое|Указывает, Корпоративный портал требуется на устройствах, зарегистрированных помощником установки, унаследованных от [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли это профилем по умолчанию|
|supervisedModeEnabled|Логический|Режим Под контролем, True, чтобы включить, ложные в противном случае. Дополнительные сведения см. [в Microsoft Intune](/mem/intune/enrollment) устройствах регистрации.|
|supportDepartment|Строка|Сведения отдела поддержки|
|isMandatory|Boolean|Указывает, является ли профиль обязательным|
|locationDisabled|Логическое|Указывает, отключена ли панорама установки службы расположения|
|supportPhoneNumber|Строка|Номер телефона поддержки|
|profileRemovalDisabled|Boolean|Указывает, отключен ли параметр удаления профиля|
|restoreBlocked|Логический|Указывает, заблокирована ли настройка области восстановления|
|appleIdDisabled|Boolean|Указывает, отключена ли области установки apple id|
|termsAndConditionsDisabled|Логическое|Указывает, отключено ли области установки "Условия и условия"|
|touchIdDisabled|Логическое|Указывает, отключена ли настройка сенсорного id|
|applePayDisabled|Boolean|Указывает, отключена ли система установки apple pay|
|siriDisabled|Boolean|Указывает, отключено ли области настройки siri|
|diagnosticsDisabled|Boolean|Указывает отключение области настройки диагностики|
|displayToneSetupDisabled|Логический|Указывает, отключен ли экран настройки displaytone|
|privacyPaneDisabled|Логический|Указывает, отключен ли экран конфиденциальности|
|screenTimeScreenDisabled|Логическое|Указывает, отключена ли установка расстановки времени на экране|
|deviceNameTemplate|Строка|Задает буквальный или имя шаблон.|
|configurationWebUrl|Boolean|URL-адрес входа помощника установки|

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




