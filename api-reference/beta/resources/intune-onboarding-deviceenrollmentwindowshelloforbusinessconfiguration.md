---
title: Тип ресурса deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Параметры Windows Hello для бизнеса позволяют пользователям получать доступ к своим устройствам с помощью жестов, таких как биометрическая проверка подлинности или ПИН-код. Настройка параметров для зарегистрированных Windows 10, Windows 10 Mobile и более поздних версий.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 906d68a7e11e94002a5b5f90b3a458c17c0cb1ad
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455059"
---
# <a name="deviceenrollmentwindowshelloforbusinessconfiguration-resource-type"></a>Тип ресурса deviceEnrollmentWindowsHelloForBusinessConfiguration

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Параметры Windows Hello для бизнеса позволяют пользователям получать доступ к своим устройствам с помощью жестов, таких как биометрическая проверка подлинности или ПИН-код. Настройка параметров для зарегистрированных Windows 10, Windows 10 Mobile и более поздних версий.


Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список объектов deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-list.md)|Коллекция [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Список свойств и связей объектов [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Получение объекта deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-get.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Чтение свойств и связей объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Создание объекта deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-create.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Создание объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Удаление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-delete.md)|Нет|Удаляет объект [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|
|[Обновление объекта deviceEnrollmentWindowsHelloForBusinessConfiguration](../api/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration-update.md)|[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)|Обновление свойств объекта [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Уникальный идентификатор для учетной записи, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|displayName|Строка|Отображаемое имя конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|description|String|Описание конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|priority|Int32|Priority используется, когда пользователь существует в нескольких группах, которым назначена Настройка регистрации. Пользователи подчиняются только конфигурации с наименьшим значением приоритета. Наследуется от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|createdDateTime|DateTimeOffset|Созданная Дата и время в формате UTC для настройки регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|lastModifiedDateTime|DateTimeOffset|Дата и время последнего изменения конфигурации регистрации устройств, унаследованной от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|version|Int32|Версия конфигурации регистрации устройств, унаследованная от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|
|pinMinimumLength|Int32|Определяет минимальное количество символов, необходимое для ПИН-кода Windows Hello для бизнеса.  Это значение должно находиться в диапазоне от 4 до 127 включительно, и меньше или равно значению, заданному для максимального ПИН-кода.|
|pinMaximumLength|Int32|Управляет максимальным количеством символов для ПИН-кода Windows Hello для бизнеса. Это значение должно находиться в диапазоне от 4 до 127 включительно. Это значение должно быть больше или равно значению, заданному для минимального ПИН-кода.|
|pinUppercaseCharactersUsage|[виндовшеллофорбусинесспинусаже](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использования прописных букв в ПИН-коде Windows Hello для бизнеса.  Allows разрешает использование прописных букв (s), в то время как это необходимо. Если задано значение "не разрешено", прописные буквы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinLowercaseCharactersUsage|[виндовшеллофорбусинесспинусаже](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использования строчных букв в ПИН-коде Windows Hello для бизнеса.  Allows разрешает использование строчных букв (s), в то время как это необходимо. Если задано значение "не разрешено", буквы нижнего регистра не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|pinSpecialCharactersUsage|[виндовшеллофорбусинесспинусаже](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|Управляет возможностью использования специальных символов в ПИН-коде Windows Hello для бизнеса.  Allows разрешает использование специальных символов, в то время как они необходимы для их отображения. Если задано значение "не разрешено", Специальные символы не будут разрешены. Возможные значения: `allowed`, `required`, `disallowed`.|
|state|[Включение](../resources/intune-shared-enablement.md)|Определяет, разрешено ли настраивать устройство для Windows Hello для бизнеса. Если задано значение Disabled, пользователь не сможет подготовить Windows Hello для бизнеса, за исключением того, что в Azure Active Directory присоединяются мобильные телефоны, если это необходимо. Если задано значение не задано, Intune не будет переопределять значения по умолчанию для клиента. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|securityDeviceRequired|Логическое|Определяет, требуется ли доверенный ПЛАТФОРМЕНный модуль для подготовки Windows Hello для бизнеса. TPM предоставляет дополнительные преимущества безопасности, которые хранятся на нем, не могут использоваться на других устройствах. Если задано значение false, все устройства могут подготавливать Windows Hello для бизнеса, даже если нет пригодного к использованию доверенного платформенного модуля.|
|unlockWithBiometricsEnabled|Логическое|Управляет использованием биометрических жестов, таких как лицо и отпечаток, в качестве альтернативы ПИН-коду Windows Hello для бизнеса.  Если задано значение false, биометрические жесты не разрешены. Пользователи по-прежнему должны настроить ПИН-код в качестве резервной копии в случае сбоев.|
|remotePassportEnabled|Boolean|Управляет использованием удаленного Windows Hello для бизнеса. Удаленная функция Windows Hello для бизнеса обеспечивает возможность использования портативного, зарегистрированного устройства в качестве вспомогательного для проверки подлинности на настольных компьютерах. Рабочий стол должен быть присоединен к Azure AD, а на вспомогательном устройстве должен быть ПИН-код Windows Hello для бизнеса.|
|pinPreviousBlockCount|Int32|Управляет возможностью запретить пользователям использовать прошлые контакты. Он должен иметь значение от 0 до 50 включительно, а текущий ПИН-код пользователя включен в этот счетчик. Если задано значение 0, предыдущие ПИН-коды не сохраняются. История ПИН-кодов не сохраняется при сбросе ПИН-кода.|
|pinExpirationInDays|Int32|Определяет период времени (в днях), в течение которого можно использовать ПИН-код, прежде чем система потребует от пользователя изменить его. Должно быть задано значение от 0 до 730 включительно. Если задано значение 0, срок действия ПИН-кода пользователя никогда не истекает|
|enhancedBiometricsState|[Включение](../resources/intune-shared-enablement.md)|Управляет возможностью использования функций защиты от спуфинга для распознавания лиц на поддерживающих его устройствах. Если задано значение Disabled, функции защиты от спуфинга не допускаются. Если задано значение не задано, пользователь может выбрать, следует ли использовать функцию защиты от спуфинга. Возможные значения: `notConfigured`, `enabled`, `disabled`.|
|секуритикэйфорсигнин|[Включение](../resources/intune-shared-enablement.md)|Ключ безопасности для входа предоставляет возможность удаленного включения и ВЫКЛЮЧЕНия функции Windows Hello Серкурити Кэйл, которые не настроены, будут поддерживать конфигурации, выполненные в Клинет. Возможные значения: `notConfigured`, `enabled`, `disabled`.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)|Список назначений групп для профиля конфигурации устройства, унаследованного от [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024,
  "pinMinimumLength": 1024,
  "pinMaximumLength": 1024,
  "pinUppercaseCharactersUsage": "String",
  "pinLowercaseCharactersUsage": "String",
  "pinSpecialCharactersUsage": "String",
  "state": "String",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 1024,
  "pinExpirationInDays": 1024,
  "enhancedBiometricsState": "String",
  "securityKeyForSignIn": "String"
}
```



