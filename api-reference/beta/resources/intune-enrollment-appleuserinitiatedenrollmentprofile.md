---
title: Тип ресурса Апплеусеринитиатеденроллментпрофиле
description: Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 108abd8668d6c863f876a0188ea48085a722e281
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528348"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a>Тип ресурса Апплеусеринитиатеденроллментпрофиле

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Ресурс объекта enrollmentprofile представляет коллекцию конфигураций, которым необходимо предоставить предварительную регистрацию, чтобы включить регистрацию определенных устройств, удостоверения которых были предварительно настроены. Для этого типа профиля назначаются идентификаторы предварительно подготовленных устройств, чтобы применить конфигурации профиля при регистрации соответствующего устройства.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Апплеусеринитиатеденроллментпрофилес](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|Коллекция [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|Список свойств и связей объектов [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .|
|[Получение Апплеусеринитиатеденроллментпрофиле](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|Чтение свойств и связей объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .|
|[Создание Апплеусеринитиатеденроллментпрофиле](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|Создание нового объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .|
|[Удаление Апплеусеринитиатеденроллментпрофиле](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|Нет|Удаляет объект [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).|
|[Обновление Апплеусеринитиатеденроллментпрофиле](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|Обновление свойств объекта [апплеусеринитиатеденроллментпрофиле](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .|
|[Действие setPriority](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|Нет|Н/Д|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|дефаултенроллменттипе|[appleUserInitiatedEnrollmentType](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|Тип регистрации профиля по умолчанию. Возможные значения: `unknown`, `device`, `user`.|
|аваилаблинроллменттипеоптионс|Коллекция [апплеовнертипинроллменттипе](../resources/intune-enrollment-appleownertypeenrollmenttype.md)|Список доступных параметров типа регистрации|
|id|Строка|GUID объекта|
|displayName|Строка|Имя профиля|
|description|String|Описание профиля|
|priority|Int32|Приоритет, 0 — самый высокий|
|platform|[девицеплатформтипе](../resources/intune-shared-deviceplatformtype.md)|Платформа устройства. Возможные значения: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.|
|createdDateTime|DateTimeOffset|Время создания профиля|
|lastModifiedDateTime|DateTimeOffset|Время последнего изменения профиля|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|assignments|Коллекция [апплинроллментпрофилеассигнмент](../resources/intune-enrollment-appleenrollmentprofileassignment.md)|Список назначений для этого профиля.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleUserInitiatedEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "String",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "String",
      "enrollmentType": "String"
    }
  ],
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "platform": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



