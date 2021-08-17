---
title: тип ресурса userAppInstallStatus
description: Содержит свойства для состояния установки для пользователя.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4df870536093a2cf47caa62fae9bb098a545d6f1e3735446f144243492c41ff2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54183298"
---
# <a name="userappinstallstatus-resource-type"></a>тип ресурса userAppInstallStatus

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния установки для пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список userAppInstallStatuses](../api/intune-apps-userappinstallstatus-list.md)|[коллекция userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Список свойств и связей [объектов userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)|
|[Get userAppInstallStatus](../api/intune-apps-userappinstallstatus-get.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Чтение свойств и связей [объекта userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)|
|[Создание userAppInstallStatus](../api/intune-apps-userappinstallstatus-create.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Создание нового [объекта userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)|
|[Удаление userAppInstallStatus](../api/intune-apps-userappinstallstatus-delete.md)|Нет|Удаляет [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).|
|[Обновление userAppInstallStatus](../api/intune-apps-userappinstallstatus-update.md)|[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)|Обновление свойств объекта [userAppInstallStatus.](../resources/intune-apps-userappinstallstatus.md)|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userName|String|Имя пользователя.|
|userPrincipalName|String|Имя главного пользователя.|
|installedDeviceCount|Int32|Количество установленных устройств.|
|failedDeviceCount|Int32|Количество устройств со сбоями.|
|notInstalledDeviceCount|Int32|Количество не установленных устройств.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|приложение|[mobileApp](../resources/intune-shared-mobileapp.md);|Ссылка на навигацию в мобильном приложении.|
|deviceStatuses|[коллекция mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Состояние установки приложения на устройствах.|

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




