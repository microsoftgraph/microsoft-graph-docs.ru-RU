---
title: Тип ресурса Депенроллментбасепрофиле
description: Ресурс Депенроллментбасепрофиле представляет профиль регистрации программы регистрации устройств Apple (DEP). Этот тип профиля должен быть назначен серийным номерам Apple DEP, прежде чем соответствующие устройства смогут регистрироваться с помощью функции DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 611df6a0aff2c2d3c0d6728aa9bbaa443d772a35
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328069"
---
# <a name="depenrollmentbaseprofile-resource-type"></a>Тип ресурса Депенроллментбасепрофиле

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

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
|рекуиресусераусентикатион|Boolean|Указывает, требуется ли для профиля проверка подлинности пользователей, унаследованных от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|конфигуратионендпоинтурл|String|URL-адрес конечной точки конфигурации, используемый для регистрации, унаследованный от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала. Наследуется от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|рекуирекомпанипорталонсетупассистантенролледдевицес|Boolean|Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке, наследуемых от [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|
|isDefault|Boolean|Указывает, является ли этот профиль профилем по умолчанию|
|супервиседмодинаблед|Boolean|Защищенный режим, true для включения, false в противном случае. Дополнительную https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune информацию можно узнать в статье.|
|суппортдепартмент|String|Сведения о отделе поддержки|
|пасскодедисаблед|Boolean|Указывает, отключена ли область настройки секретного кода|
|Обязательный|Boolean|Указывает, является ли профиль обязательной|
|локатиондисаблед|Boolean|Указывает, отключена ли область настройки службы расположения|
|суппортфоненумбер|String|Номер телефона службы поддержки|
|профилеремовалдисаблед|Boolean|Указывает, отключен ли параметр удаления профиля|
|рестореблоккед|Boolean|Указывает, заблокирована ли область настроек восстановления|
|апплеиддисаблед|Boolean|Указывает, отключена ли область настройки Apple ID|
|термсандкондитионсдисаблед|Boolean|Указывает, отключена ли область установки "условия и условия"|
|таучиддисаблед|Boolean|Указывает, отключена ли панель настройки сенсорного экрана|
|апплепайдисаблед|Boolean|Указывает, отключена ли область настройки оплаты Apple|
|зумдисаблед|Boolean|Указывает, отключена ли область настройки масштабирования|
|сиридисаблед|Boolean|Указывает, отключена ли область настройки Siri|
|диагностиксдисаблед|Boolean|Указывает, отключена ли область настройки диагностики|
|дисплайтонесетупдисаблед|Boolean|Указывает, отключен ли экран установки дисплайтоне|
|приваципанедисаблед|Boolean|Указывает, отключен ли экран конфиденциальности|
|девиценаметемплате|String|Задает шаблон литерала или имени.|

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
  "privacyPaneDisabled": true,
  "deviceNameTemplate": "String"
}
```



