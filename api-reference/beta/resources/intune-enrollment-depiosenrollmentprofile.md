---
title: Тип ресурса Депиосенроллментпрофиле
description: Ресурс Депиосенроллментпрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP), характерный для конфигурации iOS. Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 739d8bc495cebbc00837b325f68002a5ee8e9903
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328041"
---
# <a name="depiosenrollmentprofile-resource-type"></a>Тип ресурса Депиосенроллментпрофиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс Депиосенроллментпрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP), характерный для конфигурации iOS. Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.


Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Депиосенроллментпрофилес](../api/intune-enrollment-depiosenrollmentprofile-list.md)|Коллекция [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md)|Список свойств и связей объектов [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Получение Депиосенроллментпрофиле](../api/intune-enrollment-depiosenrollmentprofile-get.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Чтение свойств и связей объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Создание Депиосенроллментпрофиле](../api/intune-enrollment-depiosenrollmentprofile-create.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Создание нового объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .|
|[Удаление Депиосенроллментпрофиле](../api/intune-enrollment-depiosenrollmentprofile-delete.md)|Нет|Удаляет объект [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md).|
|[Обновление Депиосенроллментпрофиле](../api/intune-enrollment-depiosenrollmentprofile-update.md)|[depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md)|Обновление свойств объекта [депиосенроллментпрофиле](../resources/intune-enrollment-depiosenrollmentprofile.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта, наследуемого от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|displayName|Строка|Имя профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|description|String|Описание профиля, унаследованного от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|рекуиресусераусентикатион|Boolean|Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|конфигуратионендпоинтурл|String|URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала. Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|рекуирекомпанипорталонсетупассистантенролледдевицес|Boolean|Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли этот профиль профилем по умолчанию, унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|супервиседмодинаблед|Boolean|Защищенный режим, true для включения, false в противном случае. Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье. Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|суппортдепартмент|String|Сведения о отделе поддержки, унаследованные от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|пасскодедисаблед|Boolean|Указывает, является ли область настройки секретного кода наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|Обязательный|Boolean|Указывает, является ли профиль обязательно унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|локатиондисаблед|Boolean|Указывает, является ли область настроек службы расположений наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|суппортфоненумбер|String|Номер телефона поддержки, наследуемый от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|профилеремовалдисаблед|Boolean|Указывает, является ли параметр удаления профиля унаследованным от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|рестореблоккед|Boolean|Указывает, заблокирована ли область настройки "восстановление" из [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|апплеиддисаблед|Boolean|Указывает, является ли область настроек Apple ID унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|термсандкондитионсдисаблед|Boolean|Указывает, отключена ли область установки "условия и условия" от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|таучиддисаблед|Boolean|Указывает, является ли область настроек сенсорного экрана наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|апплепайдисаблед|Boolean|Указывает, отключена ли область настройки оплаты Apple от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|зумдисаблед|Boolean|Указывает, является ли область настройки масштаба унаследованной от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|сиридисаблед|Boolean|Указывает, наследуется ли область настройки Siri от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|диагностиксдисаблед|Boolean|Указывает, является ли область настройки диагностики неактивной, наследуемой от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|дисплайтонесетупдисаблед|Boolean|Указывает, отключен ли экран установки дисплайтоне от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|приваципанедисаблед|Boolean|Указывает, отключен ли экран конфиденциальности, унаследованный от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|девиценаметемплате|String|Задает шаблон литерала или имени. Наследуется от [депенроллментбасепрофиле](../resources/intune-enrollment-depenrollmentbaseprofile.md)|
|iTunesPairingMode|[iTunesPairingMode](../resources/intune-enrollment-itunespairingmode.md).|Указывает режим связывания iTunes. Возможные значения: `disallow`, `allow`, `requiresCertificate`.|
|манажементцертификатес|Коллекция [манажементцертификатевиссумбпринт](../resources/intune-enrollment-managementcertificatewiththumbprint.md)|Сертификаты управления для конфигуратора Apple|
|ресторефромандроиддисаблед|Boolean|Указывает, отключено ли восстановление из Android|
|аваитдевицеконфигуредконфирматион|Boolean|Указывает, должно ли устройство ждать настройки подтверждения.|
|Свойства sharedipadmaximumusercount|Int32|Указывает максимальное количество пользователей, которые могут использовать общий iPad. Относится только к общему режиму iPad.|
|Enablesharedipad к|Boolean|Указывает, следует ли зарегистрировать устройство в режиме, позволяющем использовать сценарии с несколькими пользователями. Применяется только в общих iPad.|
|компанипорталвпптокенид|String|Если этот параметр установлен, указывает, какой токен VPP должен использоваться для развертывания корпоративного портала с лицензией "на устройство". для задания этого свойства необходимо задать значение "enableAuthenticationViaCompanyPortal".|
|енаблесинглеаппенроллментмоде|Boolean|Указывает, что устройство включает один режим приложения и применяет блокировку приложений во время регистрации. Значение по умолчанию — false. для задания этого свойства должно быть задано значение "enableAuthenticationViaCompanyPortal" и "Компанипорталвпптокенид".|
|хомебуттонскриндисаблед|Boolean|Указывает, отключен ли экран "чувствительность к домашней кнопке"|
|имессажеандфацетимескриндисаблед|Boolean|Указывает, отключен ли экран iMessage и FaceTime|
|онбоардингскриндисаблед|Boolean|Указывает, отключен ли встроенный экран установки|
|скринтимескриндисаблед|Boolean|Указывает, отключена ли настройка времени ожидания экрана|
|симсетупскриндисаблед|Boolean|Указывает, отключен ли экран Симсетуп|
|софтвареупдатескриндисаблед|Boolean|Указывает, отключено ли обязательное экранное обновление софваре|
|ватчмигратионскриндисаблед|Boolean|Указывает, отключен ли экран контрольных значений для миграции|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depIOSEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "deviceNameTemplate": "String",
  "iTunesPairingMode": "String",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "String",
      "certificate": "String"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 1024,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "String",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```



