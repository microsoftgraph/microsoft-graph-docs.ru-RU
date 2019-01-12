---
title: Тип ресурса userAppInstallStatus
description: Содержит свойства для состояние установки для пользователя.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f17a504537b1230de175e033779441627f5f98be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938015"
---
# <a name="userappinstallstatus-resource-type"></a>Тип ресурса userAppInstallStatus

> **Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены. Использование этих API в производственных приложениях не поддерживается.

> **Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.

Содержит свойства для состояние установки для пользователя.
## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) коллекции|Свойства списка и связей объектов [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Получение userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Чтение свойства и связи объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Создание userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Создание нового объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|
|[Удаление userAppInstallStatus](../api/intune-apps-userappinstallstatus-delete.md)|Нет|Удаляет [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[Обновление userAppInstallStatus](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Обновление свойства объекта [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|String|Ключ объекта.|
|userName|String|Имя пользователя.|
|userPrincipalName|String|Имя участника-пользователя.|
|installedDeviceCount|Int32|Количество установленных устройств.|
|failedDeviceCount|Int32|Количество устройств со сбоями.|
|notInstalledDeviceCount|Int32|Количество не установленных устройств.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|приложение|[mobileApp](../resources/intune-apps-mobileapp.md);|Навигационная ссылка для мобильного приложения.|
|deviceStatuses|[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) коллекции|Состояние установки приложений на устройствах.|

## <a name="json-representation"></a>Представление JSON
Ниже представлено описание ресурса в формате JSON.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userAppInstallStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "String (identifier)",
  "userName": "String",
  "userPrincipalName": "String",
  "installedDeviceCount": 1024,
  "failedDeviceCount": 1024,
  "notInstalledDeviceCount": 1024
}
```





