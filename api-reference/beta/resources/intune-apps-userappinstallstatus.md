---
title: Тип ресурса Усераппинсталлстатус
description: Содержит свойства для состояния установки пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 951685d7acef566ab4761bc97906d5dc4b50ea6f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491024"
---
# <a name="userappinstallstatus-resource-type"></a>Тип ресурса Усераппинсталлстатус

Пространство имен: Microsoft. Graph

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния установки пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усераппинсталлстатусес](../api/intune-apps-userappinstallstatus-list.md)|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список свойств и связей объектов [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .|
|[Получение Усераппинсталлстатус](../api/intune-apps-userappinstallstatus-get.md)|[усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Чтение свойств и связей объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .|
|[Создание Усераппинсталлстатус](../api/intune-apps-userappinstallstatus-create.md)|[усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Создание нового объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .|
|[Удаление Усераппинсталлстатус](../api/intune-apps-userappinstallstatus-delete.md)|Нет|Удаляет объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md).|
|[Обновление Усераппинсталлстатус](../api/intune-apps-userappinstallstatus-update.md)|[усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Обновление свойств объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userName|String|Имя пользователя.|
|userPrincipalName|String|Имя участника пользователя.|
|installedDeviceCount|Int32|Количество установленных устройств.|
|failedDeviceCount|Int32|Количество устройств со сбоями.|
|notInstalledDeviceCount|Int32|Количество не установленных устройств.|

## <a name="relationships"></a>Связи
|Связь|Тип|Описание|
|:---|:---|:---|
|программы|[mobileApp](../resources/intune-shared-mobileapp.md);|Ссылка навигации на мобильное приложение.|
|deviceStatuses|Коллекция [mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)|Состояние установки приложения на устройствах.|

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



