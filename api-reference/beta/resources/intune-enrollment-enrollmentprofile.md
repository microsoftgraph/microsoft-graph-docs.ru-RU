---
title: Тип ресурса объекта enrollmentprofile
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4b7d2683baed89505280d8866132ce9e7846bbc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259818"
---
# <a name="enrollmentprofile-resource-type"></a>Тип ресурса объекта enrollmentprofile

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список enrollmentProfiles](../api/intune-enrollment-enrollmentprofile-list.md)|Коллекция [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md)|Список свойств и связей объектов [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Получение объекта enrollmentprofile](../api/intune-enrollment-enrollmentprofile-get.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Чтение свойств и связей объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Создание объекта enrollmentprofile](../api/intune-enrollment-enrollmentprofile-create.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Создание нового объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Удаление объекта enrollmentprofile](../api/intune-enrollment-enrollmentprofile-delete.md)|Нет|Удаляет объект [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md).|
|[Обновление объекта enrollmentprofile](../api/intune-enrollment-enrollmentprofile-update.md)|[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md);|Обновление свойств объекта [объекта enrollmentprofile](../resources/intune-enrollment-enrollmentprofile.md) .|
|[Действие setDefaultProfile](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|Нет|Н/Д|
|[функция функция exportmobileconfig](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|String|Экспорт конфигурации мобильного устройства|
|[Действие updateDeviceProfileAssignment](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|GUID объекта|
|displayName|String|Имя профиля|
|description|String|Описание профиля|
|рекуиресусераусентикатион|Boolean|Указывает, требуется ли для профиля проверка подлинности пользователя|
|конфигуратионендпоинтурл|String|URL-адрес конечной точки конфигурации, используемый для регистрации|
|enableAuthenticationViaCompanyPortal|Boolean|Указывает на проверку подлинности с помощью помощника по настройке Apple, а не корпоративного портала.|
|рекуирекомпанипорталонсетупассистантенролледдевицес|Boolean|Указывает, что корпоративный портал необходим на зарегистрированных устройствах помощника по настройке|

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




