---
title: Тип ресурса mobileAppInstallSummary
description: Содержит свойства для установки сведениям о мобильных приложений.
author: tfitzmac
ms.openlocfilehash: d998e0fe5b136afe7aa18741c5c91fcde9adcc37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314786"
---
# <a name="mobileappinstallsummary-resource-type"></a>Тип ресурса mobileAppInstallSummary

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для установки сведениям о мобильных приложений.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Получение mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-get.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Чтение свойства и связи объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .|
|[Обновление mobileAppInstallSummary](../api/intune-apps-mobileappinstallsummary-update.md)|[mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md);|Обновление свойства объекта [mobileAppInstallSummary](../resources/intune-apps-mobileappinstallsummary.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
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

## <a name="relationships"></a>Связи
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





