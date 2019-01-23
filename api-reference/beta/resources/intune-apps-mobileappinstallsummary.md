---
title: Тип ресурса mobileAppInstallSummary
description: Содержит свойства для установки сведениям о мобильных приложений.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a2bd7c30c1b00e83731766bcd80f9a9fafd8e8b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416715"
---
# <a name="mobileappinstallsummary-resource-type"></a>Тип ресурса mobileAppInstallSummary

> **Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для установки сведениям о мобильных приложений.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Чтение свойства и связи объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .|
|[Обновление mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Обновление свойства объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|installedDeviceCount|Int32|Количество устройств, которые были успешно установлены этого приложения.|
|failedDeviceCount|Int32|Количество устройств, которые не удалось установить это приложение.|
|notApplicableDeviceCount|Int32|Количество устройств, которые не применимы для этого приложения.|
|notInstalledDeviceCount|Int32|Количество устройств, для которого не установлено приложение.|
|pendingInstallDeviceCount|Int32|Количество устройств, которые были уведомлены для установки этого приложения.|
|installedUserCount|Int32|Число пользователей, чьи устройств успешно для установки этого приложения.|
|failedUserCount|Int32|Число пользователей, имеющих 1 или другие устройства, который не удалось установить это приложение.|
|notApplicableUserCount|Int32|Число пользователей, которых устройства не все для этого приложения.|
|notInstalledUserCount|Int32|Число пользователей, которые имеют 1 или более устройства, на которых не установлено приложение.|
|pendingInstallUserCount|Int32|Число пользователей, имеющих 1 или другие устройства, уведомлены для установки этого приложения и 0 устройств со сбоями.|

## <a name="relationships"></a>Отношения
Нет

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppInstallSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppInstallSummary",
  "id": "String (identifier)",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "notInstalledDeviceCount": 1024,
  "pendingInstallDeviceCount": 1024,
  "installedUserCount": 1024,
  "failedUserCount": 1024,
  "notApplicableUserCount": 1024,
  "notInstalledUserCount": 1024,
  "pendingInstallUserCount": 1024
}
```




