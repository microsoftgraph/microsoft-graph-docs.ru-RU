---
title: Тип ресурса Секуритиконфигуратионтаск
description: Задача настройки безопасности.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: eaf2f479d491e8d6455dc3b296053a84983fdf98
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/18/2020
ms.locfileid: "46793501"
---
# <a name="securityconfigurationtask-resource-type"></a>Тип ресурса Секуритиконфигуратионтаск

Пространство имен: microsoft.graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Задача настройки безопасности.


Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Секуритиконфигуратионтаскс](../api/intune-partnerintegration-securityconfigurationtask-list.md)|Коллекция [секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md)|Список свойств и связей объектов [секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md) .|
|[Получение Секуритиконфигуратионтаск](../api/intune-partnerintegration-securityconfigurationtask-get.md)|[секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md)|Чтение свойств и связей объекта [секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md) .|
|[Создание Секуритиконфигуратионтаск](../api/intune-partnerintegration-securityconfigurationtask-create.md)|[секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md)|Создание нового объекта [секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md) .|
|[Удаление Секуритиконфигуратионтаск](../api/intune-partnerintegration-securityconfigurationtask-delete.md)|Нет|Удаляет объект [секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md).|
|[Обновление Секуритиконфигуратионтаск](../api/intune-partnerintegration-securityconfigurationtask-update.md)|[секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md)|Обновление свойств объекта [секуритиконфигуратионтаск](../resources/intune-partnerintegration-securityconfigurationtask.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|displayName|String|Имя. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|description|String|Описание. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|createdDateTime|DateTimeOffset|Дата создания. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|dueDateTime|DateTimeOffset|Дата выполнения. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|category|[deviceAppManagementTaskCategory](../resources/intune-partnerintegration-deviceappmanagementtaskcategory.md)|Категория. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `unknown`, `advancedThreatProtection`.|
|priority|[deviceAppManagementTaskPriority](../resources/intune-partnerintegration-deviceappmanagementtaskpriority.md)|Приоритет. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `none`, `high`, `low`.|
|модуль|String|Адрес электронной почты создателя. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|креаторнотес|String|Заметки автора. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|assignedTo|String|Имя или электронная почта администратора, которому назначена эта задача. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md)|
|status|[deviceAppManagementTaskStatus](../resources/intune-partnerintegration-deviceappmanagementtaskstatus.md)|Состояние. Наследуется от [девицеаппманажементтаск](../resources/intune-partnerintegration-deviceappmanagementtask.md). Возможные значения: `unknown`, `pending`, `active`, `completed`, `rejected`.|
|ендпоинтсекуритиполици|[ендпоинтсекуритиконфигуратионтипе](../resources/intune-partnerintegration-endpointsecurityconfigurationtype.md)|Тип политики безопасности конечной точки. Возможные значения: `unknown`, `antivirus`, `diskEncryption`, `firewall`, `endpointDetectionAndResponse`, `attackSurfaceReduction`, `accountProtection`.|
|аппликаблеплатформ|[ендпоинтсекуритиконфигуратионаппликаблеплатформ](../resources/intune-partnerintegration-endpointsecurityconfigurationapplicableplatform.md)|Соответствующая платформа. Возможные значения: `unknown`, `macOS`, `windows10AndLater`, `windows10AndWindowsServer`.|
|ендпоинтсекуритиполиципрофиле|[ендпоинтсекуритиконфигуратионпрофилетипе](../resources/intune-partnerintegration-endpointsecurityconfigurationprofiletype.md)|Профиль политики безопасности конечной точки. Возможные значения: `unknown` , `antivirus` ,,,,, `windowsSecurity` `bitLocker` `fileVault` `firewall` `firewallRules` ,,, `endpointDetectionAndResponse` `deviceControl` `appAndBrowserIsolation` , `exploitProtection` , `webProtection` , `applicationControl` , `attackSurfaceReductionRules` , `accountProtection` .|
|insights|String|Сведения об устранении.|
|манажеддевицекаунт|Int32|Число уязвимых устройств.|
|интендедсеттингс|Коллекция [keyValuePair](../resources/intune-shared-keyvaluepair.md)|Предполагаемые параметры и их значения.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|managedDevices|Коллекция [вулнераблеманажеддевице](../resources/intune-partnerintegration-vulnerablemanageddevice.md)|Уязвимые управляемые устройства.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityConfigurationTask"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityConfigurationTask",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "dueDateTime": "String (timestamp)",
  "category": "String",
  "priority": "String",
  "creator": "String",
  "creatorNotes": "String",
  "assignedTo": "String",
  "status": "String",
  "endpointSecurityPolicy": "String",
  "applicablePlatform": "String",
  "endpointSecurityPolicyProfile": "String",
  "insights": "String",
  "managedDeviceCount": 1024,
  "intendedSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



