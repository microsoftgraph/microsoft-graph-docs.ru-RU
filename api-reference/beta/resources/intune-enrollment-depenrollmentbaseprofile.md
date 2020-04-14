---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7ca200b9212f979660956a866e5a70ad47f4599a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358851"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>Тип ресурса Депенроллментбасепрофиле

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.


Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Депенроллментбасепрофилес](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|Коллекция [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Список свойств и связей объектов [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|
|[Получение Депенроллментбасепрофиле](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)|Чтение свойств и связей объекта [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|рекуиресусераусентикатион|Логическое|Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|конфигуратионендпоинтурл|String|URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Логическое|Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала. Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|рекуирекомпанипорталонсетупассистантенролледдевицес|Логическое|Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли этот профиль профилем по умолчанию|
|супервиседмодинаблед|Логическое|Защищенный режим, true для включения, false в противном случае. Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.|
|суппортдепартмент|String|Сведения о отделе поддержки|
|пасскодедисаблед|Логическое|Указывает, отключена ли область настройки секретного кода|
|Обязательный|Логическое|Указывает, является ли профиль обязательной|
|локатиондисаблед|Логическое|Указывает, отключена ли область настройки службы расположения|
|суппортфоненумбер|String|Номер телефона службы поддержки|
|профилеремовалдисаблед|Логическое|Указывает, отключен ли параметр удаления профиля|
|рестореблоккед|Логическое|Указывает, заблокирована ли область настроек восстановления|
|апплеиддисаблед|Логическое|Указывает, отключена ли область настройки Apple ID|
|термсандкондитионсдисаблед|Логическое|Указывает, отключена ли область установки "условия и условия"|
|таучиддисаблед|Логическое|Указывает, отключена ли панель настройки сенсорного экрана|
|апплепайдисаблед|Логическое|Указывает, отключена ли область настройки оплаты Apple|
|зумдисаблед|Логическое|Указывает, отключена ли область настройки масштабирования|
|сиридисаблед|Логическое|Указывает, отключена ли область настройки Siri|
|диагностиксдисаблед|Логическое|Указывает, отключена ли область настройки диагностики|
|дисплайтонесетупдисаблед|Логическое|Указывает, отключен ли экран установки дисплайтоне|
|приваципанедисаблед|Логическое|Указывает, отключен ли экран конфиденциальности|
|скринтимескриндисаблед|Логическое|Указывает, отключена ли настройка времени ожидания экрана|
|девиценаметемплате|String|Задает шаблон литерала или имени.|
|конфигуратионвебурл|Логическое|URL-адрес для входа в помощнике по настройке|

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
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "String",
  "configurationWebUrl": true
}
```



