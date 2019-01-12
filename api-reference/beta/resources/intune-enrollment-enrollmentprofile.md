---
title: Тип ресурса enrollmentProfile
description: Ресурс enrollmentProfile представляет коллекцию конфигураций, которым необходимо предоставить предварительной регистрации для включения регистрация некоторых устройствах, идентификаторы были предварительно разделены. Предварительно разделены устройства удостоверения назначаются этот тип профиля для применения настроек профиля в регистрации соответствующего устройства.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b88745c060e71e32199a96b23f94fa0d3229d451
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935593"
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
|[функция exportMobileConfig](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|Строка|Экспорт конфигурации мобильных устройств|
|[Действие updateDeviceProfileAssignment](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|GUID объекта|
|displayName|Строка|Имя профиля|
|описание|Строка|Описание профиля|
|requiresUserAuthentication|Логический|Указывает необходимость проверки подлинности пользователей в профиле|
|configurationEndpointUrl|Строка|URL-адрес конечной точки конфигурации для подачи заявок|
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





