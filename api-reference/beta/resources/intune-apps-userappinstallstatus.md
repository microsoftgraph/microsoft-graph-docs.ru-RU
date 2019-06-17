---
title: Тип ресурса Усераппинсталлстатус
description: Содержит свойства для состояния установки пользователя.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 60049701413605396ee4bf8d7277a02a11cc5bc0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993300"
---
# <a name="userappinstallstatus-resource-type"></a>Тип ресурса Усераппинсталлстатус

> **Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.

> **Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Содержит свойства для состояния установки пользователя.

## <a name="methods"></a>Методы
|Метод|Возвращаемый тип|Описание|
|:---|:---|:---|
|[Список Усераппинсталлстатусес](../api/intune-apps-userappinstallstatus-list.md)|Коллекция [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Список свойств и связей объектов [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .|
|[Получение Усераппинсталлстатус](../api/intune-apps-userappinstallstatus-get.md)|[Усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Чтение свойств и связей объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .|
|[Создание Усераппинсталлстатус](../api/intune-apps-userappinstallstatus-create.md)|[Усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Создание нового объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .|
|[Удаление Усераппинсталлстатус](../api/intune-apps-userappinstallstatus-delete.md)|Нет|Удаляет объект [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md).|
|[Обновление Усераппинсталлстатус](../api/intune-apps-userappinstallstatus-update.md)|[Усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md)|Обновление свойств объекта [усераппинсталлстатус](../resources/intune-apps-userappinstallstatus.md) .|

## <a name="properties"></a>Свойства
|Свойство|Тип|Описание|
|:---|:---|:---|
|id|Строка|Ключ объекта.|
|userName|String|Имя пользователя.|
|userPrincipalName|String|Имя участника пользователя.|
|installedDeviceCount|Int32|Количество установленных устройств.|
|failedDeviceCount|Int32|Количество устройств со сбоями.|
|notInstalledDeviceCount|Int32|Количество не установленных устройств.|

## <a name="relationships"></a>Отношения
|Отношение|Тип|Описание|
|:---|:---|:---|
|программы|[mobileApp](../resources/intune-apps-mobileapp.md);|Ссылка навигации на мобильное приложение.|
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





