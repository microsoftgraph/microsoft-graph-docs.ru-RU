---
title: Тип ресурса enrollmentProfile
description: Ресурс enrollmentProfile представляет коллекцию конфигураций, которым необходимо предоставить предварительной регистрации для включения регистрация некоторых устройствах, идентификаторы были предварительно разделены. Предварительно разделены устройства удостоверения назначаются этот тип профиля для применения настроек профиля в регистрации соответствующего устройства.
ms.openlocfilehash: 884fee5c6851e79d96cd036294e5e5485d6df66a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27078466"
---
# <a name="enrollmentprofile-resource-type"></a>Тип ресурса enrollmentProfile

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

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
|описание|String|Описание профиля|
|requiresUserAuthentication|Логический|Указывает необходимость проверки подлинности пользователей в профиле|
|configurationEndpointUrl|String|URL-адрес конечной точки конфигурации для подачи заявок|
|enableAuthenticationViaCompanyPortal|Логический|Указывает на проверку подлинности с Apple помощник по настройке вместо портала компании.|

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
  "enableAuthenticationViaCompanyPortal": true
}
```





